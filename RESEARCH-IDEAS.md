# Research ideas for *Energy Economics* SI — "The Role of Geopolitics in Energy Markets"

**Prepared:** 22 October 2026
**Target:** Elsevier *Energy Economics*, special issue 334954, guest editors **Lutz Kilian, Michael D. Plante, Siquan Wang**
**Constraint set:** Latin America preferred (not binding), econometrics must be strong enough to survive this editorial team.

---

## 0. Before anything else: verify the call

I could not open the ScienceDirect page from this environment (the network policy returns 403 for `sciencedirect.com`), so the following comes from search summaries and **must be confirmed on the journal page or by emailing the guest editors**:

| Item | What I found | Confidence |
|---|---|---|
| Journal | *Energy Economics* | High |
| Guest editors | Kilian, Plante, Wang | High |
| Scope | Geopolitical energy **supply disruptions**, with explicit interest in the Iran War and the closure of the Strait of Hormuz (late Feb 2026, ~20% of global oil/LNG flows); editors state they want "questions and practical problems not commonly considered in the literature" | Medium-high |
| Deadline | **Conflicting**: 30 Jun 2026 (lapsed), 2 Nov 2026, 15 Jan 2027, 31 Jul 2027 appear on different Elsevier pages | **Low — resolve this first** |

**Action:** email the guest editors with a 150-word abstract of your top pick and ask (a) the operative deadline and (b) whether the question is in scope. With Kilian co-editing, a pre-submission inquiry is cheap and the answer is informative. If the window is Nov 2026, idea #2 or #5 below (fastest data) is the only realistic shortlist; if it is Jan/Jul 2027, idea #1 is the right swing.

---

## 1. The editorial filter (this drives the rankings more than novelty does)

This is not a generic *Energy Economics* submission. The guest editors' own research programme defines the acceptance frontier:

**Rewarded**
- Physical-market realism: barrels, inventories, spare capacity, refinery runs, ton-miles, takeaway capacity. Quantities, not just prices.
- Credible identification of a *named* shock — narrative dating, external instruments, high-frequency windows, structural VARs with defensible restrictions.
- Measurement contributions and parameters the literature has to *assume* (short-run supply elasticity above all).
- Pass-through to gasoline prices, inflation, and inflation expectations (Kilian–Zhou's own agenda).
- Policy objects that actually exist: strategic reserve releases, sanctions licences, price-smoothing funds, subsidy rules.

**Penalised (treat as near-automatic rejection risk)**
- A geopolitical-risk *index* on the right-hand side of a return regression. GPR/EPU-as-regressor papers are the single most crowded and least credible genre in this space.
- TVP-VAR "connectedness"/spillover tables, Diebold–Yilmaz variance-decomposition indices, wavelet coherence, quantile-on-quantile, NARDL for its own sake, GARCH volatility-spillover papers.
- "Oil price" as a scalar shock with no decomposition into supply vs. demand vs. precautionary-demand components.
- Event studies on daily returns with no economic mechanism and no quantity evidence.
- Local projections used loosely (generated regressors, no lag-augmentation, SEs that ignore the instrument's estimation error).

Kilian's *Facts and Fiction in Oil Market Modeling* (*Energy Economics* 110, 2022) is the explicit statement of the methodological standard he applies — read it as the referee report you will receive, and pre-empt it in your identification section. Also read Kilian & Zhou on oil-market VAR econometrics, Känzig (2021, *AER*) for the oil-supply-news instrument, and Baumeister–Hamilton for the Bayesian-prior counter-position so you can cite both sides without picking a fight.

**Design implication:** build the paper around a *shock you can name and date*, an *outcome you can measure in physical units*, and a *parameter the literature needs*. All five shortlisted ideas are constructed to that template.

---

## 2. The event landscape (your identification capital)

Facts from reporting, each to be re-verified against a primary source before you cite it:

- **Iran War from 28 Feb 2026**; Strait of Hormuz effectively closed since; described as the largest energy supply disruption on record. Brent spiked ~50% to near $120, then traded wildly ($80s to $112) through Oct 2026 on reopening rumours. As of 22 Oct 2026 the strait is reportedly still closed.
- **Gulf producers (Saudi, UAE, Kuwait, Iraq) cut production** because barrels had nowhere to go — a supply disruption that is simultaneously a *landlocked-surplus* event. Unusual and under-theorised.
- **IEA considered the largest coordinated stock release in its history.**
- **Venezuela, Dec 2025–Feb 2026:** regime change (reporting conflicts on the exact timing and mechanism — S&P says removal ~Dec 2025, a trade outlet says capture in early Jan 2026 plus a naval blockade), then US sanctions easing, expanded Chevron authorisation, and export licences for Vitol and Trafigura. Output recovering to ~1.1–1.2 mb/d by mid-2026, a seven-year high. **This is a second, opposite-signed, LatAm geopolitical supply shock, dated weeks before the war.**
- **Latin America as the residual supplier:** Rystad-sourced reporting puts South American government revenue ~$43bn above the pre-war baseline for 2026 (Petrobras ~$13.1bn); Brazil exporting >3 mb/d with little short-run headroom; Argentina at a record ~887 kb/d from Vaca Muerta; Brazil, Guyana, Venezuela and Colombia selling more crude at better prices than at any point this decade.
- **Latin America as victim:** Chile, Peru, Central America and the Caribbean import nearly all fuel. **Mexico's refined-product import bill exceeded its crude export earnings in early 2026 for the first time in ≥36 years.** Brazil sources ~40% of fertiliser through Hormuz.

The two-sided structure — LatAm exporters gaining, LatAm importers losing, within one region sharing a data environment — is the comparative advantage of a Latin America paper for this issue. Sell it that way: not "a LatAm case study," but "a region that contains both the margin of global supply response and the most exposed importers."

---

## 3. The long list: 18 ideas, scored

Scores 1–5. **Fit** = probability this editorial team wants it (weight 0.40); **Feasibility** = data access + completable before deadline (0.35); **Novelty** = 0.25.

| # | Idea (one line) | Fit | Feas | Nov | Weighted |
|---|---|---|---|---|---|
| **1** | **Short-run supply elasticity of LatAm oil, well-level, identified off the Hormuz shock** | 5 | 4 | 5 | **4.65** |
| **2** | **Venezuela's reopening + the war: two opposite-signed supply shocks and state-dependent price responses** | 5 | 4 | 5 | **4.65** |
| **3** | **Fuel-price stabilisation funds under a tail shock: pass-through, fiscal liability, inflation counterfactuals (LAC panel)** | 5 | 5 | 4 | **4.75** |
| **4** | **LNG shock × hydrology → electricity prices and industrial output (BR/AR/CL)** | 4 | 4 | 5 | **4.25** |
| **5** | **The end of the petro-peso: Mexico's sign flip from oil winner to oil loser (+ the sovereign hedge)** | 4 | 5 | 4 | **4.35** |
| 6 | Fertiliser through Hormuz → Brazilian planting decisions and food prices (municipal shift-share) | 3 | 3 | 5 | 3.50 |
| 7 | Chokepoint-to-chokepoint: Hormuz rerouting meets Panama Canal capacity (slot-auction prices as scarcity measure) | 4 | 3 | 5 | 3.90 |
| 8 | Can the Western Hemisphere reroute? Ton-miles, freight, and destination reallocation of LatAm crude | 4 | 4 | 4 | 4.00 |
| 9 | Oil news and inflation expectations in EMs: daily Focus/Banxico survey identification | 4 | 5 | 3 | 4.10 |
| 10 | Station-level rockets-and-feathers in Mexico (~13k stations, daily) under the war shock + IEPS offset | 4 | 4 | 3 | 3.75 |
| 11 | Strategic reserves without an SPR: LAC days-of-cover and the incidence of the IEA release | 4 | 3 | 4 | 3.65 |
| 12 | Sovereign spreads in LAC: who pays the geopolitical premium (exporters vs. importers)? | 3 | 5 | 2 | 3.45 |
| 13 | Distributional incidence of the 2026 shock across LAC households (microsimulation) | 3 | 4 | 4 | 3.60 |
| 14 | Diesel pass-through to freight tariffs and regional food CPI (Brazil) | 3 | 3 | 3 | 3.00 |
| 15 | Oil windfalls, institutions and resource nationalism: does a price spike change contracts? | 3 | 2 | 4 | 2.90 |
| 16 | Caribbean/Central American power tariffs with fuel-cost pass-through clauses | 3 | 2 | 4 | 2.90 |
| 17 | Argentina LNG FIDs as real options under geopolitical risk | 2 | 3 | 4 | 2.85 |
| 18 | Lithium triangle / transition-mineral geopolitics | 2 | 4 | 2 | 2.70 |

Ideas 15–18 are dropped: 15 and 16 have weak power and messy policy coding, 17 is a few-events calibration rather than econometrics, 18 risks being judged out of scope for an oil/gas-disruption issue.

---

## 4. The five

### #1 — How elastic is Latin American oil supply? Well-level evidence from the Hormuz shock
**Recommended if your deadline is 2027. This is the highest-value paper on the list.**

**Question.** Oil-market SVARs *must* take a stand on the short-run price elasticity of supply, and the entire Kilian–Murphy vs. Baumeister–Hamilton debate turns on it. Credible micro estimates exist essentially only for US shale (Newell–Prest, Bjørnland et al.). Nobody has estimated it for Vaca Muerta or Brazilian pre-salt — which in 2026 is precisely where the marginal non-OPEC barrel was supposed to come from. You answer a parameter question the literature is forced to assume, using the largest exogenous price shock on record.

**Shock.** Hormuz closure is as close to exogenous-to-LatAm-supply as this literature ever gets: a war elsewhere, LatAm producers are price takers. Construct the instrument two ways: (i) Känzig-style oil supply news shocks from futures-curve revisions around narratively dated war/escalation announcements; (ii) a pure narrative indicator for the Feb 28 window and subsequent escalations. Report both.

**Data (all believed free and granular — verify first).**
- **Argentina:** Secretaría de Energía open data — monthly **well-level** production (oil/gas by well, operator, basin, formation) plus the fracture/completion dataset (stage counts, lateral length, sand). Portal `datos.energia.gob.ar` was unreachable from this environment; confirm dataset names and vintages.
- **Brazil:** ANP monthly production by field and well; drilling and concession data.
- **Colombia:** ANH/Ecopetrol field-level monthly. **Guyana:** no granular data — handle as an aggregate case study, not a panel unit.

**Specification.** Two margins, separately.
1. *Extensive (drilling/completions).* Operator × basin × month panel. Local projections with lag augmentation:
   $y_{i,t+h} - y_{i,t-1} = \alpha_i^h + \beta^h \varepsilon_t^{oil} + \gamma^h(L)X_{i,t-1} + u_{i,t+h}$, $h = 0,\dots,18$, where $\varepsilon^{oil}$ is the identified supply news shock. Two-way clustered SEs; Driscoll–Kraay for cross-sectional dependence; bootstrap the instrument's first-stage estimation error into the bands.
2. *Intensive (output from existing wells).* Fit pre-shock type curves by vintage cohort and formation, then test for post-shock deviations from predicted decline (choke management, workovers, refrac). This is where "elasticity" is usually overstated by aggregate studies, so separating it is itself a contribution.

**Mechanism and heterogeneity — this is what makes it publishable rather than a regression.** Interact with **takeaway capacity** (Oldelval/Vaca Muerta Sur pipeline utilisation), operator liquidity and foreign ownership, and Argentina's contemporaneous policy regime (RIGI incentives, FX regime). Show the elasticity is a *capacity-constrained* object: the answer to "can the Western Hemisphere replace Hormuz barrels?" is an engineering constraint with an economic shadow price, and you can estimate it.

**Why it lands.** Closes with a direct message to the SVAR literature: here is the out-of-sample, non-US short-run supply elasticity, here is how it compares to the priors your models impose, here is what it implies for the price response to a chokepoint closure. Kilian cares about that parameter more than about Latin America, and you give him both.

**Risks.** (a) Argentine policy changes confound — mitigate with Brazil as the policy-stable comparison and with event-window tightness. (b) Anticipation: pre-trends from the 2025 ramp-up — control with cohort fixed effects and pre-shock trend tests. (c) Dataset access; verify in week 1 before committing.

---

### #2 — Two geopolitical supply shocks, one month apart: Venezuela's reopening and the Hormuz closure
**Highest-novelty option. First-mover on the 2026 Venezuelan reopening.**

**Question.** Within six weeks, world oil supply received a *positive* geopolitically-driven shock (Venezuelan sanctions relief, ~+0.5 mb/d, dated Jan–Feb 2026) and a *negative* one roughly thirty times larger (Hormuz). Is the price response per barrel symmetric? Theory says no: with inventories drawn and spare capacity stranded behind a closed strait, the price response per lost barrel should be far larger in the war state. You estimate that state dependence using two cleanly dated, opposite-signed, *geopolitical* shocks — not a GARCH asymmetry, a structural one.

**Identification.**
- Narrative dating from OFAC/Treasury licence actions (general licence amendments, the Vitol/Trafigura authorisations) for the relief shock; the Jan–Feb window is clean of the war, which starts 28 Feb.
- High-frequency windows on futures (intraday if you can get it; daily settlements otherwise) around announcement timestamps.
- A structural oil-market VAR in which both events enter as identified supply shocks, with the war shock allowed a state-dependent coefficient (inventory cover / OECD days-of-supply as the state variable). Historical decomposition and counterfactual paths.

**Quantities, which is what sells it.** Heavy-sour differentials (Maya formula price, WCS–WTI, Mars–WTI from CME settlements), **EIA weekly US crude imports by country of origin**, **PADD 3 refinery crude inputs and utilisation**, USGC crack spreads, Venezuelan output from OPEC MOMR secondary sources cross-checked against Chevron's 10-Q disclosures. Add a synthetic control for Venezuelan output (donor pool of sanctioned/recovering producers) to measure the reopening itself.

**Risks.** Venezuelan data quality is genuinely poor — be explicit and use bounds rather than point estimates for output. Political reversal risk during review. Few events means you must lean on the structural model, not the event study, for the headline number.

---

### #3 — Who pays for smoothing? Fuel-price stabilisation funds under a tail geopolitical shock
**Safest high-fit option; fastest to a complete draft. Recommended if the deadline is near.**

**Question.** Latin America is the world's densest laboratory of fuel-price smoothing rules: Colombia's FEPC, Chile's MEPCO, Peru's FEPC, Ecuador's subsidy bands, Bolivia's fixed prices, Mexico's variable IEPS stimulus, Brazil's discretionary Petrobras pricing policy. A disruption of this size is exactly the state in which these rules were never stress-tested. Three results, all policy-relevant and none standard: (i) pass-through of the international product price to the pump under each regime, including asymmetry; (ii) the *contingent fiscal liability* the rules generated — an implicit short option on oil that these states wrote and that the war exercised; (iii) counterfactual CPI paths had each country used its neighbour's rule.

**Why the editors like it.** Retail pass-through and oil-to-inflation transmission is the guest editors' own literature (Kilian–Zhou on gasoline prices, inflation and expectations). "Practical problems not commonly considered" is literally the call's language, and the fiscal-option framing is not in the energy literature.

**Data (weekly/monthly, public).** Brazil ANP weekly station survey (municipality-level, survey microdata); Chile CNE weekly; Colombia MinMinas/Ecopetrol; Peru Osinergmin *Facilito*; Mexico CRE price reports plus the weekly IEPS stimulus published in the *DOF*; Uruguay URSEA/ANCAP. International benchmarks: **USGC conventional gasoline and ULSD spot from EIA (free)** — use *product* prices, not crude, or a referee will object correctly. Fiscal cost from budget-execution reports and FEPC/MEPCO statements. CPI weights from each statistics office.

**Specification.** Country-level ECM in the Borenstein–Cameron–Gilbert tradition with regime interactions:
$\Delta p^{retail}_{c,t} = \sum_j (\theta_j^+ \Delta x^+_{c,t-j} + \theta_j^- \Delta x^-_{c,t-j}) + \lambda(p^{retail}_{c,t-1} - \mu_c - \nu_c x_{c,t-1}) + \delta' (\text{regime}_c \times \Delta x_{c,t}) + \text{FE} + \epsilon$
with a threshold/state-dependent version (shock size above the historical 95th percentile) to test whether smoothing rules break under tail shocks. Then (a) a fiscal-liability calculation from the realised wedge × volumes, and (b) synthetic-control inflation counterfactuals across regimes. Cluster by country, bootstrap with few clusters (wild cluster bootstrap — with ~8 countries this matters, say so before the referee does).

**Risks.** Few clusters → inference discipline required. Regime changes mid-sample (several countries altered rules in 2026) — this is a feature if you date them narratively, a fatal flaw if you ignore them. Brazil's pricing policy is discretionary, not a rule; treat it as a separate category.

---

### #4 — Qatari LNG, Andean hydrology, and the price of electricity
**Best pure-identification paper on the list.**

**Question.** Hormuz carried roughly a fifth of global LNG. South America's power systems are hydro-dominated with gas/diesel at the margin, so the same global gas shock hits a country hard or barely at all depending on the hydrological state — which is plausibly exogenous. That interaction identifies the pass-through of a geopolitical gas shock into electricity prices, thermal dispatch and industrial output, with a credible first stage and high-frequency data.

**Design.** Plant-level dispatch and system spot prices at daily/hourly frequency:
$y_{p,t} = \beta_1 \varepsilon^{gas}_t + \beta_2 H_{t} + \beta_3 (\varepsilon^{gas}_t \times H_{t}) + \text{plant FE} + \text{week FE} + \text{controls} + u_{p,t}$
where $H$ is reservoir inflow/storage relative to the historical distribution and $\varepsilon^{gas}$ is the identified global gas shock. $\beta_3$ is the object of interest. Then a second stage on real outcomes: electricity-intensity shift-share across manufacturing sectors (monthly industrial production by sector) and the CPI electricity component.

**Data.** Brazil: ONS (natural energy inflows, reservoir levels, dispatch), CCEE PLD spot, ANEEL tariff flags. Argentina: CAMMESA hourly dispatch and costs, ENARSA LNG tender awards (public prices — a useful free substitute for JKM). Chile: Coordinador Eléctrico hourly marginal cost and dispatch, GNL Quintero. **Watch out:** JKM is paywalled; pre-identify your gas-price series (TTF, Henry Hub from EIA, plus tender awards) before you commit, and be explicit about the measurement issue rather than hiding it.

**Risks.** Hydrology and global gas prices can be correlated through global weather/El Niño — control for ENSO indices and test. Regulated tariffs mute pass-through to consumers: measure that explicitly as a result (it becomes a second contingent-liability story, linking to #3).

---

### #5 — The end of the petro-peso: Mexico's flip from oil winner to oil loser
**Most quotable; lowest execution risk; strong macro-finance econometrics.**

**Question.** Mexico has been the textbook oil-exporting commodity currency for forty years. By early 2026 its refined-product import bill exceeded crude export earnings for the first time in at least thirty-six years. The 2026 shock is therefore the first instance in which a geopolitical oil-supply shock should *hurt* Mexico. Test it: has the sign of the oil-price beta of the peso, the sovereign spread, the terms of trade and the fiscal balance flipped?

**Specification.** Not a scalar oil price — decompose. Känzig-style oil supply news shocks plus a Kilian-style supply/aggregate-demand/precautionary-demand decomposition; then state-dependent local projections with the net-oil-position state, plus structural break tests with unknown break date (Andrews QLR, Bai–Perron, and a Bayesian time-varying-parameter version as robustness *only*). Outcomes: MXN/USD, EMBI/ICE spreads, terms of trade, oil fiscal revenue, Pemex's quasi-fiscal position, gasoline-import volumes.

**The hook referees will remember:** **Mexico's sovereign oil hedge.** The Hacienda buys put options every year; 2026 is the realisation in which the hedge was supposed to pay off — and in which the country's net exposure had already flipped, so the hedge was partly hedging a risk Mexico no longer runs. Price the programme against the realised path, compute the ex-post payoff versus premium, and ask whether a product-import hedge now dominates a crude-export put. That is a genuinely new policy question, and strikes, volumes and premiums are published in SHCP documents with a lag.

**Data.** Banxico, INEGI, SHCP, Pemex financial reports and export volumes, EIA product exports to Mexico, CME options data for hedge valuation. All free.

**Risks.** Break tests have low power on short post-break samples — be upfront, and complement with the structural/state-dependent approach rather than resting on a break date. Confounded by Mexico-specific 2026 policy; include a Colombia/Brazil comparison panel.

---

## 5. Wildcards worth a second look

- **#6 Fertiliser through Hormuz → Brazilian agriculture.** Municipal shift-share (crop mix × fertiliser intensity × Hormuz-origin import exposure) on planted area, crop switching and yields, using Comex Stat imports by HS code/origin/port and IBGE PAM/LSPA. The most "not commonly considered" idea on the list and a clean energy→food geopolitics link (urea and ammonia are gas-derived, so it *is* an energy paper). Held out of the five only because the 2026/27 planting response is only now observable — if your deadline is Jul 2027, promote it.
- **#7 Chokepoint interaction: Hormuz and Panama.** The Panama Canal publishes transit data and **slot-auction clearing prices**, which are a market-priced measure of chokepoint scarcity — a rare and under-used dataset. Estimate how a closure at one chokepoint prices capacity at another. High novelty, medium feasibility.
- **#9 Oil news and EM inflation expectations.** Brazil's Focus survey is high-frequency; Banxico's and Colombia's are regular. Direct extension of Kilian–Zhou to emerging markets with a tail shock. Low novelty, very high feasibility — a good "second paper" from the same data build as #3.

---

## 6. If I had to choose one

**Deadline in Jan or Jul 2027 → idea #1** (supply elasticity). It answers a parameter question the editors' own literature cannot settle, uses Latin America because that is where the marginal barrel actually is, and the well-level data make the econometrics unimpeachable. Highest expected citation value too.

**Deadline in weeks → idea #3** (stabilisation funds). Public weekly data, a clean regime-comparison design, pass-through econometrics squarely in the editors' wheelhouse, and the contingent-fiscal-option framing is new.

**Best pairing:** #3 first (fast, safe, builds the LAC price database), then #1 as the follow-up using the same regional infrastructure. #2 is the one to grab if you want the first-mover claim on Venezuela and can tolerate data risk.

---

## 7. Week-1 feasibility checks (do these before writing a word of the paper)

1. Email the guest editors: operative deadline + scope check on your top pick.
2. **Argentina:** confirm `datos.energia.gob.ar` well-level production and fracture datasets exist, their last update, and whether 2026 months are posted. (Could not verify from this environment.)
3. **Brazil:** confirm ANP well/field monthly production and the weekly fuel-price survey microdata are current through Q3 2026.
4. **Mexico:** confirm CRE station-level price data is still published and at what frequency (it was reportedly degraded from 3×/day to 1×/day years ago; a monthly state-average fallback would weaken idea #10 but not #5).
5. **Gas prices:** settle your LNG price series for idea #4 (JKM is paywalled — check institutional access; otherwise ENARSA tender awards + TTF/HH).
6. **Differentials:** check access to Maya/WCS/Mars realised prices for idea #2 (CME settlements are free; Argus/Platts assessments are not).
7. Build the narrative chronology of 2026 events now, with primary-source citations (OFAC notices, IEA statements, OPEC MOMR, national regulators). Every idea here depends on it, and a sloppy chronology is the easiest thing for a referee to attack.

## 8. Referee-proofing checklist

- Name the shock. Date it. Show the first stage.
- Decompose oil prices; never regress on a scalar "oil price" or on a GPR index.
- Report quantities alongside prices.
- Lag-augment local projections; bootstrap instrument-generated-regressor uncertainty into the bands; state your clustering and use a wild cluster bootstrap with few clusters.
- Pre-trend and placebo windows (e.g. the Jan 2026 Venezuela window as a placebo for war-shock specifications, and vice versa).
- Compare your estimate to the priors imposed in the existing SVAR literature — explicitly, with a table.
- Address Kilian (2022) head-on in the identification section rather than waiting for the referee to raise it.
