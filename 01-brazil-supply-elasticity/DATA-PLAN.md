# Data plan — Paper 1 (Brazil supply elasticity)

**Status:** specification only. **Nothing has been downloaded.** All outbound HTTP from this container is blocked by the environment's network policy, so every URL, dataset name and schema below is from prior knowledge or search summaries and carries a verification status. The machine-readable version is `code/sources.yaml`.

**Estimation sample: 2000–2025. Out-of-sample test window: Jan 2026 – latest available.**

---

## 1. Dataset inventory

### Tier 1 — the paper does not exist without these

| ID | Dataset | Agency | Unit | Freq | Coverage | Status |
|---|---|---|---|---|---|---|
| `anp_prod_well` | Produção de petróleo e gás natural **por poço** | ANP (dados abertos / Painel Dinâmico de Produção) | well | monthly | ~2000– | **Verify: well-level granularity and whether it names the production unit** |
| `anp_prod_field` | Produção **por campo** | ANP | field | monthly | ~2000– | High confidence |
| `anp_wells_registry` | Cadastro de poços / poços perfurados (SIGEP) | ANP | well | event | long | Verify format |
| `anp_units` | Instalações/plataformas de produção: **nameplate capacity + startup date** | ANP + Petrobras releases + EPE BOR | production unit | static/event | — | **Likely hand-assembled — see §3** |
| `anp_refining` | Processamento de petróleo nas refinarias | ANP | refinery | monthly | ~2000– | High confidence |
| `comex_crude_exp` | Crude exports, **HS 2709**, by destination and port, value + volume | Comex Stat (MDIC/Secex) | HS×dest×port | monthly | 1997– | High confidence |
| `brent` | Brent spot / Dated Brent | EIA (`RBRTE`) or FRED (`DCOILBRENTEU`) | — | daily | 1987– | High confidence, free |

### Tier 2 — needed for identification and controls

| ID | Dataset | Agency | Unit | Freq | Status |
|---|---|---|---|---|---|
| `bh_rigs` | International rig count, Brazil (offshore/onshore split) | Baker Hughes | country | monthly | Free, high confidence |
| `anp_gov_take` | Participações governamentais (royalties, participação especial) | ANP | field | monthly | Medium |
| `anp_sales` | Vendas de derivados | ANP | product×state | monthly | High |
| `comex_prod_imp` | Refined product imports, **HS 2710** | Comex Stat | HS×origin | monthly | High |
| `petrobras_ops` | Production and sales reports; realised export prices; capex | Petrobras IR | firm | quarterly | High |
| `petrobras_plan` | Plano Estratégico (capex plans by vintage) | Petrobras | firm | annual | High |
| `epe_bor` | Brazilian Oil & Gas Report (breakevens, field economics) | EPE | — | annual | Free PDFs, English |
| `bcb_macro` | BRL/USD, Selic, country risk | BCB SGS | — | daily/monthly | Free API |
| `futures_curve` | WTI/Brent futures curve settlements (for the shock series) | CME | contract | daily | **See §4 — main instrument risk** |

### Tier 3 — optional Argentina extension module

Kept in the manifest so it can be switched on without rework; **off by default** per your call. `ar_prod_well` (Secretaría de Energía well-level production), `ar_fractures` (completion registry), `ar_netback` (export duties, administered prices, FX gap). The netback construction is the expensive part and is the reason this module is not free.

---

## 2. Panel construction

```
anp_prod_well ──┐
anp_wells_reg ──┼─→ [well-month panel, 2000–2026]
anp_units ──────┘        │
                         ├─→ collapse → operator × basin × month   → STAGE 1 (extensive margin)
                         ├─→ well-level deviations from type curve  → STAGE 2 (intensive margin)
                         ├─→ field × month + unit nameplate         → STAGE 3 (capacity constraint)
                         └─→ national monthly                       → STAGE 4 (allocation margin)

anp_refining + comex_crude_exp + anp_prod_field → export share = exports / production
comex_crude_exp (value ÷ volume) → realised export price (free proxy for Argus/Platts assessments)
```

**Key derived variables**

| Variable | Construction | Note |
|---|---|---|
| `fpso_util` | field or unit production ÷ nameplate capacity | The central regressor in Stage 3. Requires `anp_units`. |
| `well_age`, `cohort` | months since first production; first-production year × formation | For type curves |
| `realised_export_px` | Comex Stat FOB value ÷ volume, by month | Free substitute for Tupi/Búzios assessments; coarser (monthly, blended grades) but defensible — document the limitation |
| `export_share` | crude exports ÷ domestic production | Stage 4 outcome |
| `refinery_margin` | product price basket − crude cost (EIA USGC crack as proxy) | Stage 4 regressor |
| `netback` | Brent − freight − quality diff | Brazil faces market prices, so this is far simpler than the Argentine case |

---

## 3. The one manual task that cannot be automated

**Building `anp_units`: the well-to-production-unit crosswalk with nameplate capacity and startup dates.**

The capacity-constraint identification — the paper's mechanism — needs each well linked to the floating production unit it flows to, each unit's processing nameplate, and the month it started up. If `anp_prod_well` carries an installation field, this is a join. If it does not, it must be assembled by hand from field development plans, ANP installation registries, Petrobras press releases and the EPE reports, for roughly 40–60 units.

**This is the first thing to check, and it determines the paper's design.** Please look at the ANP well-level file and tell me whether it has an installation/platform column. If it does not, the fallback is a field-level design using commissioning dates alone, which is weaker but workable.

---

## 4. The instrument: honest assessment

Stage 1 needs an oil supply news shock series through 2026.

- Känzig's replication files are public and run through roughly 2023. **They must be extended to 2026**, which means assembling OPEC and geopolitical announcement dates and the futures-curve revisions around them.
- That requires daily futures **curve** data, not just front-month. CME settlements are published, but bulk historical access is awkward and some vendors paywall it. **This is the largest unresolved feasibility risk in the paper** — larger than the ANP question, because there is no free fallback of equal quality.
- Fallbacks, in descending order of credibility: (i) front-month plus a few maturities from EIA/FRED, which loses curve detail; (ii) a pure narrative shock indicator from announcement dates, which loses the magnitude information; (iii) Caldara–Cavallo–Iacoviello-style country-level supply shocks, if their series is public and updated.

Resolve this in week 1 alongside the ANP check.

---

## 5. Verification checklist — do these before any estimation

1. `anp_prod_well` exists at well level, with coverage back to ~2000 and **through 2026**.
2. It names the **production unit** per well (decides §3).
3. Volume units (m³ vs. bbl) and whether oil and condensate are separated.
4. `days on production` is present — needed to distinguish downtime from decline.
5. Operator field is consistent over time, or a name-harmonisation crosswalk is needed (operator names change with M&A; PetroRio→Prio, etc.).
6. Comex Stat crude exports are available monthly at HS8 with destination **and** port.
7. Baker Hughes Brazil rig count has an offshore/onshore split.
8. A route to daily futures curve data exists (§4).
9. EPE BOR PDFs for 2021/22–2024/25 downloadable.
10. Petrobras quarterly production reports machine-readable, or need manual extraction.

---

## 6. Known data risks

| Risk | Severity | Response |
|---|---|---|
| No well-to-unit link in ANP data | **High** | Field-level fallback; hand-built crosswalk for major units |
| No free futures curve source | **High** | Narrative-only shock, documented as a limitation; or buy one month of vendor access |
| Operator concentration (Petrobras dominant) | **High** | Treat as the political-economy channel, not a nuisance; split Petrobras vs. private operators |
| Realised export price is monthly and blended | Medium | Document; cross-check against Petrobras reported realised prices |
| Type curves confound technology drift with price response | Medium | Cohort × formation fixed effects; test on pre-shock holdout |
| 2026 months not yet published | Medium | The out-of-sample window shortens; report what exists and state the cut-off |
| Unit nameplate capacity revised over time (debottlenecking) | Medium | Collect revisions; use the contemporaneous value, test sensitivity |
