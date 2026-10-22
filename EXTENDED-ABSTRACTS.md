# Extended abstracts: three proposals for the *Energy Economics* geopolitics SI

**Prepared:** 22 October 2026 · Companion to `RESEARCH-IDEAS.md` (long list of 19 ideas)
**Guest editors:** Lutz Kilian, Michael D. Plante, Siquan Wang

---

## Part I — Revised novelty and feasibility audit

### I.1 What I could and could not verify

**All direct HTTP is blocked from this environment.** Every data portal I tested returned 000 (`datos.energia.gob.ar`, `gov.br`, `ccee.org.br`, `cammesa`, `coordinador.cl`, `comexstat`, `ons.org.br`, `eia.gov`, `datos.gob.ar`), and ScienceDirect returns a 403 at the proxy. So:

- **Novelty claims below are search-verified** and reasonably reliable.
- **Data-existence claims are not directly verified.** They come from search results plus prior knowledge, and each is flagged. The week-1 checklist in `RESEARCH-IDEAS.md` §9 is therefore load-bearing, not boilerplate.

### I.2 The finding that should change your strategy

Searching for prior work on the 2026 shock turned up **two Dallas Fed working papers already modelling the Hormuz closure**:

- **WP 2609 (April 2026):** complete closure removing ~20% of global oil supply; quarterly WTI to ~$103 under a one-quarter closure, falling to ~$71 on reopening.
- **WP 2615 (June 2026):** a 15% net world supply decline (after diversions), benchmarked against a 5% shock described as the average of four historical disruptions; ROW real GDP growth falls ~6× the US response.
- Plus Dallas Fed public analysis (March 2026): a Q2 closure cutting global real GDP growth by ~2.9pp annualised, WTI averaging ~$98.

**Michael D. Plante is a Dallas Fed economist and a guest editor of this issue.** Read that carefully:

1. **Do not submit an aggregate scenario or macro-impact paper.** The editors' own institution has already done it, with better internal data and a head start. A paper estimating "the effect of the Hormuz closure on global prices/GDP" competes directly with the editors' work and loses.
2. **The complementary niche is micro-identified, regional, parameter-estimating work.** Those scenario models must *assume* a short-run supply elasticity and *assume* a mapping from barrels lost to price. Supplying one of those parameters from microdata is the highest-value thing an outside author can contribute to this issue — it makes the editors' own papers better rather than competing with them.
3. All three proposals below are built on that logic. Say so explicitly in your cover letter.

Also relevant: an MDPI *Sustainability* paper on the 2026 Hormuz shipping disruption already exists, but it concedes its freight and insurance figures are "illustrative operational scenario benchmarks rather than econometrically estimated causal parameters." The topic is claimed; the econometrics is not.

### I.3 Novelty, re-checked

| Idea | What exists | Verdict |
|---|---|---|
| **#1 LatAm supply elasticity** | Well-level elasticities exist **only for the US**: Bjørnland, Nordvik & Rohrer (North Dakota, 16,000+ wells, elasticity ~0.3–0.9, no conventional response); Aastveit et al., *Quantitative Economics* 2026 (both margins respond, refracs more than new completions); Anderson, Kellogg & Salant (Texas, near-zero conventional, reservoir-pressure constrained). **No published Vaca Muerta or pre-salt estimate.** The global short-run elasticity (~0.06–0.07) is *constructed* by assuming US shale is the only responsive segment — untested. A Sept 2026 commentary is already disputing a spring-2026 aggregate elasticity estimate. | **Gap confirmed, and the question is live and contested.** Highest novelty on the list. |
| **#3 Stabilisation funds** | Colombia is partly covered: *Retail Prices of Gasoline and Asymmetric Adjustment to Wholesale Prices in Colombia* (J. Econ. Development, 2022); a 2026 Springer paper decomposing Colombian retail prices into pass-through, strategic complementarities and market power (monthly, four cities, 2017–19). IMF (2023) notes MEPCO-era deviations from international prices but publishes no pass-through estimate. SEI documents the FEPC's 2022 deficit at ~2.5% of GDP. Institutional critiques of the FEPC exist. | **Novelty downgraded from v2.** Country-level asymmetric pass-through in Colombia is taken. What remains genuinely new: cross-regime comparative estimation, tail-state rule breakdown, and pricing the rule as a written option. Reposition around those. |
| **#2 Venezuela + war, state dependence** | Nothing found on the 2026 Venezuelan reopening. Nothing found estimating convexity of the price response using paired opposite-signed geopolitical shocks. | **Gap confirmed.** Highest ceiling. |
| **#4 Gas shock × hydrology → power** | No paper estimates gas-price shocks and inflows jointly for Brazil/Chile. Nearest: a 2026 arXiv preprint on optimistic inflow forecasts distorting Brazilian hydrothermal dispatch (SDDP simulation, not reduced-form) — which incidentally suggests **inflow forecast errors** as an additional instrument. Trade press is already writing "US–Iran tensions drive Chile's electricity price volatility." | Gap real but the topic is in the air; see §I.5 for why it lost the third slot. |
| **#19 Chokepoint-episode panel** | No panel-episode econometric study found. Only consultancy and tracking-firm scenario work (Kpler ton-miles, J.P. Morgan inflation estimates, Xeneta rates) and the MDPI scenario paper. | Gap confirmed, but **feasibility collapsed** — see §I.5. |

### I.4 Feasibility, re-checked

| Idea | Data position | Grade |
|---|---|---|
| **#1** | Argentine well-level production + fracture registry and Brazilian ANP well/field production are monthly, long (2009/2010→), and large (order 10⁶ well-months). Estimation sample is 2010–2025, so the eight-month problem never arises. **Single point of failure: the Argentine portal, unverifiable from here.** One substantive measurement task: Argentina's administered domestic prices, export duties and FX gap mean the price a producer faces ≠ Brent, so a producer-netback series must be constructed. That is work, not a blocker — and it is itself a contribution. | **A** |
| **#3** | Weekly retail price panels, ~25 years, multiple countries, plus a Brazilian station/municipality panel for within-country power. Rule parameters and fund balances are published. International benchmarks free from EIA. Nothing paywalled. | **A+** |
| **#2** | Prices and US-side quantities are excellent and free (CME settlements; EIA weekly imports by origin, PADD-level refinery inputs and utilisation; IEA/EIA inventories; OPEC MOMR). **The weak link is the Venezuelan barrel count**, which is load-bearing because the headline parameter is per-barrel. Handled by bounds, not assumption — see §IV.4. | **B+** |
| **#4** | Hourly power data excellent. **But JKM spot is paywalled**, and the whole design hinges on measuring the global gas shock. CME JKM futures settlements and ENARSA tender awards are workable substitutes but each is attackable, and I could not verify either. | **B** |
| **#19** | **This is what killed it.** Baltic Exchange tanker indices (BDTI/BCTI), Clarksons and Kpler/Vortexa AIS are all licensed commercial products. The historical episodes need archival freight data. Without institutional subscriptions the identification has no measured treatment intensity. | **C** |

### I.5 Re-ranking, and why these three

Weights as before: **Data 0.40, Fit 0.35, Novelty 0.25.**

| Rank | Idea | Data | Fit | Nov | Weighted |
|---|---|---|---|---|---|
| **1** | #1 LatAm supply elasticity | 5 | 5 | 5 | **5.00** |
| **2** | #3 Stabilisation funds as written options | 5 | 5 | 4 | **4.75** |
| **3** | #2 Venezuela + war, state dependence | 3.5 | 5 | 5 | **4.40** |
| 4 | #4 Gas × hydrology → power | 4.5 | 4 | 4.5 | 4.33 |
| 5 | #19 Chokepoint-episode panel | 2.5 | 4 | 4.5 | 3.53 |

**#4 lost by 0.07 and is a legitimate alternative** — I am not pretending that gap is meaningful. Two reasons it sits fourth: electricity markets are one transmission step removed from an oil-and-gas-disruption special issue, so fit is lower; and the LNG price series is paywalled, which is the one thing you told me to weight most. If you have institutional Platts/Argus access, #4 moves to second and I would swap it in.

**#19 is out on data, not ideas.** If you have Clarksons or Kpler through your institution, tell me and it returns — it has the highest ceiling of anything on the list.

The three below are also a deliberate portfolio: micro-supply (#1), micro-price plus fiscal (#3), market-level structural (#2). Different literatures, different data builds, different risk profiles. All three are oil rather than power, matching the issue's core.

---

## Part II — Proposal 1: supply elasticity

# How Elastic Is Non-U.S. Oil Supply? Well-Level Evidence from Argentina and Brazil, 2010–2026

### The main point, in one paragraph

**Every structural oil-market model and every Hormuz scenario exercise must assume a short-run price elasticity of oil supply, and that assumption is based entirely on U.S. evidence.** Well-level estimates exist for North Dakota and Texas and nowhere else; the global elasticity used in practice (~0.06–0.07) is constructed by assuming U.S. shale is the only responsive segment of world supply. This paper estimates the elasticity from microdata for the two producers that actually constitute the Western Hemisphere's supply margin — Argentine Vaca Muerta shale and Brazilian pre-salt — and shows that **the elasticity is not a geological or financial parameter but a midstream one: it is bounded above by pipeline takeaway capacity.** Argentina has U.S.-like shale geology with entirely different infrastructure and institutions, which is exactly why it identifies the constraint. The 2026 price spike, the largest in the sample by construction, is used not to estimate the elasticity but to test it out of sample: the fitted model over-predicts the observed 2026 supply response, and the gap measures the shadow value of the binding capacity constraint.

### Why this issue wants it

The guest editors' own institution has published scenario models of the Hormuz closure (Dallas Fed WP 2609, WP 2615) whose price paths depend on an assumed supply response from non-OPEC producers outside the U.S. This paper supplies that parameter from microdata. It is complementary to the editors' work rather than competing with it, and the closing section translates the estimate directly into what it implies for a 15–20% supply loss — the exact object those papers model.

### Data

| Source | Unit | Frequency | Coverage | Status |
|---|---|---|---|---|
| Argentina, Secretaría de Energía open data: well-level production | well | monthly | ~2009– | **Verify first — decisive** |
| Argentina, fracture/completion registry (lateral length, stages, proppant, fluid) | well | per-operation | ~2013– | Verify |
| Brazil, ANP: production by well and field; concession and drilling records | well/field | monthly | ~2000– | High confidence |
| Colombia, ANH/Ecopetrol field-level production (secondary panel) | field | monthly | — | Medium |
| Midstream capacity: Oldelval expansions, Vaca Muerta Sur/VMOS commissioning dates and nameplate | pipeline | event | 2010– | Company filings |
| Prices: ICE Brent, CME WTI futures curves; Känzig-style oil supply news shocks | — | daily→monthly | 1986– | High |
| Argentine policy wedge: export duties, administered domestic prices, FX gap | country | monthly | 2010– | Medium |

Panel size: order 20,000+ Argentine wells × ~180 months, plus the Brazilian field/well panel. **Estimation sample 2010–2025**, which contains the 2014–16 collapse, the 2020 COVID collapse and the 2021–22 spike. The eight-post-shock-month problem does not arise.

**Measurement task that must be done properly.** Argentina administered domestic crude prices and levied export duties through much of the sample, so the netback a producer faced is not Brent. Construct
$p^{net}_{i,t} = f(\text{Brent}_t,\ \text{export duty}_t,\ \text{domestic price control}_t,\ \text{FX gap}_t,\ \text{quality diff}_i,\ \text{transport tariff}_{b,t})$
and document it in an appendix. This is the first question a referee will ask, and done well it is a contribution — the Brazilian panel, which faces market prices, is the control for whether netback mismeasurement drives the results.

### Econometrics

**Stage 1 — extensive margin (drilling and completions).** Operator × basin × month, lag-augmented local projections:
$$y_{i,t+h} - y_{i,t-1} = \alpha_i^h + \beta^h\,\varepsilon_t + \Gamma^h(L)X_{i,t-1} + u_{i,t+h},\qquad h=0,\dots,18$$
with $y$ = log spuds, log completions, rig count, frac-crew count; $\varepsilon_t$ = identified oil supply news shock (Känzig-style, from futures-curve revisions around OPEC and geopolitical announcement dates), with a narrative-dates version as the robustness check. Inference: two-way clustering (operator, month), Driscoll–Kraay for cross-sectional dependence, and a bootstrap that propagates the first-stage estimation error of $\varepsilon_t$ into the bands — $\varepsilon_t$ is a generated regressor and ignoring that is the standard error in this literature.

**Stage 2 — intensive margin (existing wells).** Fit type curves by formation × vintage cohort on pre-shock data (Arps hyperbolic, plus a flexible spline in well age as robustness); outcome is the log deviation of realised from predicted output; regress on the shock with well fixed effects and age controls. This isolates choke management, workovers and refracs from new drilling — the margin Aastveit et al. find most responsive in the U.S., and the one aggregate studies conflate.

**Stage 3 — aggregation to an elasticity, and the capacity constraint.** Combine the two margins into an implied basin-level supply elasticity at horizon $h$. Then test the central hypothesis by interacting the shock with pre-determined midstream utilisation $U_{b,t-1}$:
$$\beta^h(U) = \beta_0^h + \beta_1^h U_{b,t-1}$$
predicting $\beta_1^h < 0$. Identify the shadow price of capacity from the netback wedge (domestic vs. export parity) as $U \to 1$, and use the staggered commissioning of Oldelval and Vaca Muerta Sur as within-sample capacity-relief events.

**Stage 4 — 2026 out of sample.** Feed the realised 2026 price path into the model fitted on 2010–2025 and compare predicted with actual output, March–October 2026, as a conditional forecast with bands. The shortfall is the capacity constraint binding, and it is a falsifiable prediction rather than a short-sample regression.

**Stage 5 — back to the structural literature.** A table comparing the estimate to the elasticity priors imposed in Kilian–Murphy and Baumeister–Hamilton, and what it implies for the price response to a 15–20% supply loss.

### What could kill it, and the mitigation

| Threat | Mitigation |
|---|---|
| Argentine portal lacks well-level data or 2026 months | **Check in week 1.** Brazilian ANP alone supports a thinner version; Colombia as a third panel. |
| Netback mismeasurement from price controls | Explicit netback construction; Brazil as market-priced control; exclude controlled periods as robustness |
| RIGI, FX unification and tax reform coincide with the 2026 window | Estimation is pre-2026, so policy contaminates only the out-of-sample test; use Brazil as the policy-stable comparison and report the test for both countries |
| Pre-trends from the 2025 ramp-up | Cohort fixed effects, explicit pre-trend tests, placebo horizons |
| Simultaneity (does LatAm supply move Brent?) | Argentina is ~0.9% of world supply; discuss and dismiss with a magnitude argument |

---

## Part III — Proposal 2: stabilisation funds

# An Implicit Short Option on Oil: Fuel-Price Smoothing Rules and the Fiscal Cost of the 2026 Disruption

### The main point, in one paragraph

**Latin American fuel-price smoothing rules are short option positions on crude, written by states to households, and the 2026 disruption exercised them.** Colombia's FEPC, Chile's MEPCO, Peru's FEPC, Ecuador's bands, Bolivia's fixed prices and Mexico's variable IEPS stimulus are usually studied as subsidy policy or as pass-through frictions. They are better understood as derivatives: each rule defines a state-contingent payoff from the sovereign as a function of the international price, with a strike, a notional (national fuel consumption) and no hedge. This paper estimates pass-through under each rule over roughly twenty-five years of weekly data, shows that **the rules break non-linearly in the tail** — pass-through jumps once the international shock exceeds the 95th–99th percentile of its historical distribution, as fiscal capacity rather than the rule starts to bind — and then prices the option: what the 2026 disruption cost each sovereign ex post, and what the ex-ante fair premium would have been at pre-war implied volatilities.

### Why this issue wants it

Pass-through from international prices to the pump, and onward to inflation, is the guest editors' own research agenda. The call asks for practical problems not commonly considered: the contingent fiscal liability embedded in fuel-price rules is a real one, it is currently being realised across the region at a scale of percent of GDP, and no one has priced it. It also gives the issue a fiscal-transmission channel for geopolitical shocks that the macro papers will not cover.

### Positioning against what exists (novelty, honestly)

Country-level asymmetric pass-through in Colombia is already published (J. Econ. Development, 2022; and a 2026 Springer paper decomposing Colombian retail prices into cost pass-through, strategic complementarities and market power using monthly data for four cities, 2017–19). The IMF has noted that Chilean retail prices deviated from international prices after MEPCO began operating in its current form in 2014, but published no estimate. SEI puts the FEPC's 2022 deficit at ~2.5% of GDP.

So the contribution is **not** "rockets and feathers in Latin America." It is: (i) the first comparative estimation across smoothing regimes on a common weekly sample and a common international benchmark; (ii) the first test of **tail-state rule breakdown**; (iii) the option-pricing framing, which makes the fiscal cost comparable across countries whose rules have entirely different mechanics. State those three contributions in the abstract and cite the Colombian papers prominently — a referee who knows them and does not see them cited will reject.

### Data

| Source | Unit | Frequency | Coverage | Status |
|---|---|---|---|---|
| **Brazil ANP fuel-price survey** (the long spine) | station / municipality | weekly | ~2001– | High confidence; verify history depth |
| Chile CNE price reports; ENAP estimated-price reports | national / region | weekly | ~2000s– | Medium-high |
| Colombia MinMinas / Ecopetrol regulated price structure | city | monthly/weekly | — | Medium |
| Peru Osinergmin *Facilito* | station | daily/weekly | — | Medium |
| Mexico CRE station prices; weekly IEPS stimulus in the *DOF* | station / national | daily / weekly | — | Medium-high |
| Uruguay URSEA/ANCAP; Ecuador; Bolivia (administered) | national | monthly | — | Medium |
| **International benchmark: USGC conventional gasoline and ULSD spot (EIA)** | — | daily | 1986– | High, free |
| Rule parameters: MEPCO weekly parameters, FEPC balances, fund reports, budget execution | country | weekly/quarterly | — | Medium |
| Volumes (option notional): national fuel sales | country | monthly | — | Medium-high |
| CPI weights and fuel subindices | country | monthly | — | High |

Panel: ~6–8 countries × ~1,250 weeks, plus the Brazilian station panel (thousands of stations × weekly) as the high-powered within-country anchor. **Use product prices, not crude, as the benchmark** — a referee will correctly object otherwise.

### Econometrics

**1. Pass-through baseline.** Country-by-country asymmetric error-correction model in the Borenstein–Cameron–Gilbert tradition, estimated on 2001–2025:
$$\Delta p^{ret}_{c,t} = \sum_{j=0}^{J}\left(\theta_j^{+}\Delta x^{+}_{c,t-j} + \theta_j^{-}\Delta x^{-}_{c,t-j}\right) + \lambda_c\left(p^{ret}_{c,t-1} - \mu_c - \nu_c x_{c,t-1}\right) + \delta_c' Z_{c,t} + \epsilon_{c,t}$$
with $x$ the import-parity product price in local currency (so the FX channel is explicit), and $Z$ covering taxes and rule parameters. Report cumulative asymmetry $\sum\theta^+ - \sum\theta^-$ and the half-life of adjustment by regime.

**2. Tail-state rule breakdown — the core test.** Threshold/smooth-transition ECM with transition variable $s_{c,t} = $ the percentile of $|\Delta x_{c,t}|$ in its own historical distribution:
$$\Delta p^{ret}_{c,t} = G(s_{c,t};\gamma,\kappa)\,\Theta_{tail}'W_{c,t} + \left[1-G(s_{c,t};\gamma,\kappa)\right]\Theta_{norm}'W_{c,t} + \epsilon_{c,t}$$
Test $H_0:\Theta_{tail}=\Theta_{norm}$ with Hansen threshold tests and bootstrapped p-values; estimate $\kappa$ rather than imposing it. **The 2026 observations are the tail realisations that identify $\Theta_{tail}$ jointly with 2008, Libya 2011 and Russia 2022** — which is precisely how a recent shock should enter a short-sample design.

**3. Regime comparison and inference discipline.** Pooled specification with regime × shock interactions. With ~8 clusters, conventional cluster-robust inference is invalid: use wild cluster bootstrap and report randomisation inference. Carry the Brazilian station-level panel as the internal-validity anchor where clustering does not bind. Date every 2026 rule change narratively — several countries altered rules mid-year, which is additional identifying variation if dated and a fatal confound if ignored. Brazil's Petrobras pricing is discretionary, not a rule: separate category throughout.

**4. Option valuation — the novel core.** Write each rule's sovereign cash flow as a payoff function of the international price:
$$\Pi_{c,t} = -\max\left\{x_{c,t} - \bar{p}_{c,t},\,0\right\}\times Q_{c,t}$$
where $\bar p$ is the rule-implied domestic reference and $Q$ is volume. Compute (i) the **realised 2026 payout** per country as a share of GDP and of fiscal revenue; (ii) the **ex-ante fair premium** by Monte Carlo on an oil-price process estimated pre-war, with and without a geopolitical jump component calibrated to pre-war option-implied skew. The spread between realised payout and ex-ante premium is the mispricing the war revealed. Report sensitivity to the jump intensity — this is where a referee will push, so lead with it.

**5. Inflation counterfactual.** Feed counterfactual pump-price paths (each country under each other country's rule) through CPI weights with estimated second-round effects, and run synthetic-control comparisons of headline inflation across smoothing regimes.

### What could kill it, and the mitigation

| Threat | Mitigation |
|---|---|
| Colombian pass-through already published | Reposition on the three stated contributions; cite the existing work prominently |
| Few clusters | Wild cluster bootstrap, randomisation inference, Brazilian station panel as anchor |
| Endogenous rule choice (countries with volatile politics adopt smoothing) | Acknowledge; the option-valuation and tail-breakdown results are accounting and within-regime, not cross-regime causal claims. Do not over-claim causality here |
| Rules changed during 2026 | Narrative dating; treat as variation |
| Volumes and fund balances published with lags or gaps | Bound the liability; report ranges |

---

## Part IV — Proposal 3: two shocks

# Thirty Barrels to One: State Dependence in the Price Response to Geopolitical Supply Shocks

### The main point, in one paragraph

**Early 2026 delivered two geopolitically driven oil supply shocks of opposite sign, radically different size, and six weeks apart — and their comparison identifies the convexity that linear oil-market models assume away.** Venezuelan sanctions relief added roughly half a million barrels a day from a standing start in January–February 2026; the Hormuz closure removed 15–20% of world supply from 28 February. Because both are geopolitical rather than demand-driven, both are narratively datable, and they are close enough in time that inventories, market structure and the macro state are otherwise comparable, the pair identifies **how the price response per barrel depends on whether spare capacity is physically reachable.** Gulf producers held ample spare capacity throughout 2026 — stranded behind a closed strait. The paper estimates a strongly convex mapping from barrels to price and shows that scenario models using a linear mapping understate the price response to a chokepoint closure while overstating the relief from marginal supply additions.

### Why this issue wants it

Every scenario exercise, the editors' own included, must map a quantity of lost supply into a price. Dallas Fed WP 2615 benchmarks a 15% net decline against a 5% shock described as the average of four historical disruptions — an implicitly linear comparison. If the mapping is convex in the state of accessible spare capacity, that scaling is wrong in a knowable direction and by an estimable amount. This is the most direct possible contribution to the issue's core question, and the Venezuelan reopening is a first-mover topic nobody has written on.

### Data

| Source | Unit | Frequency | Coverage | Status |
|---|---|---|---|---|
| ICE Brent, CME WTI, Mars, WCS settlements and full futures curves | contract | daily | long | High, free |
| CME options: implied vol and skew (precautionary-demand proxy) | contract | daily | long | High |
| **EIA weekly US crude imports by country of origin** (the clean Venezuelan observable) | origin | weekly | 2010– | High, free |
| EIA PADD-level refinery inputs, utilisation, product supplied | PADD | weekly | long | High, free |
| OECD and US commercial inventories; SPR; IEA release volumes | region | weekly/monthly | long | High |
| OPEC MOMR secondary-source production; announced Gulf cuts | country | monthly | long | High |
| OFAC/Treasury licence actions and amendments (dated, with text) | event | event | Dec 2025–2026 | High |
| Chevron 10-Q Venezuela disclosures; Vitol/Trafigura authorisations | firm | quarterly/event | 2026 | High |
| **War-news event chronology: 30–60 dated events, Feb–Oct 2026** | event | daily | 2026 | **Must be built** |

### Econometrics

**1. High-frequency event study (Archetype C).** Daily — intraday where obtainable — changes in futures levels and curve shape around dated events, classified as escalation, de-escalation, reopening signal, or policy response (IEA release, OPEC action). Separate coefficients for Venezuela-relief events and war events. Exclude or control for overlapping macro release days. The Jan–Feb relief window is clean of the war, which begins 28 February: protect that by dating precisely.

**2. External-instrument SVAR.** Monthly oil-market VAR in production, inventories, real activity and the real price, identified with the high-frequency shock series as an external instrument (proxy SVAR / SVAR-IV), estimated 1985–2026. This supplies the long sample that eight months of 2026 cannot.

**3. State dependence — the core specification.** Interact the identified supply shock with a pre-determined state variable $S_{t-1}$ combining **accessible** spare capacity (OPEC spare capacity net of volumes stranded behind the closure) and days of commercial inventory cover:
$$y_{t+h} = \alpha^h + \left[\beta_0^h + \beta_1^h S_{t-1}\right]\varepsilon_t^{supply} + \Gamma^h(L)X_{t-1} + u_{t+h}$$
estimated as state-dependent local projections and, as a cross-check, a smooth-transition SVAR. Test convexity ($\beta_1^h \neq 0$) and report the implied per-barrel price response at the 2026 state versus the sample-median state. Bootstrap inference must propagate the generated-instrument uncertainty.

**4. Bounds instead of assumptions on the Venezuelan barrels.** Venezuelan output is poorly measured and the parameter is per-barrel, so the denominator is the weak link. Do not pick a number. Bracket it: the lower bound from **EIA observed US imports from Venezuela** (barrels actually delivered, cleanly measured, weekly), the upper bound from the **OPEC secondary-source output change** (total production response, including non-US destinations). Report the per-barrel elasticity across the whole interval and show the convexity conclusion holds throughout. Turning the data weakness into transparent bounds is more persuasive than hiding it in a calibration — and it pre-empts the obvious referee objection.

**5. Falsification.** The Jan–Feb Venezuela window as a placebo for war-shock specifications and vice versa; pre-trend tests; a test for war anticipation using pre-28-February option skew; exclusion of days with major macro releases.

**6. Payoff section.** Re-run a Dallas Fed-style closure scenario substituting the estimated convex mapping for a linear one, and report how much the predicted price and GDP paths change. That is the sentence the editors will quote.

### What could kill it, and the honest limitation

| Threat | Mitigation |
|---|---|
| Venezuelan barrel count | Bounds, as above. This is the design's main vulnerability and must be addressed in the abstract, not an appendix |
| **The extreme state is a single episode** | Unavoidable and must be stated plainly: the long sample disciplines the curve over most of its range, but the estimate *at the 2026 state* is identified off one realisation. Report it as such, with the historical disruptions (1973, 1979, 1990, 2022) as the comparison set. This is your eight-month objection resurfacing in a different form — it does not sink the paper, but it must be confessed rather than buried |
| Conflicting reports on Venezuelan regime-change timing | Resolve against primary sources before dating anything; the Dec 2025 vs Jan 2026 discrepancy in the secondary reporting is unresolved |
| Political reversal during review | Frame the contribution as the parameter, not the forecast |
| Event-set construction is subjective | Pre-register the classification rules; report results under alternative event sets; have a second coder |

---

## Part V — Recommendation

**Write #1.** It has the best data position, the clearest gap in the literature, the most defensible econometrics, and it is complementary to rather than competitive with the editors' own Hormuz work. Its single point of failure is one dataset, which you can check in an afternoon.

**If that check fails, write #3.** Nothing in it is paywalled, the estimation sample is twenty-five years long, and the option-pricing framing is new enough to carry the paper even though Colombian pass-through is taken.

**Write #2 if you want the highest-ceiling paper** and are comfortable defending a per-barrel parameter whose denominator is bounded rather than measured.

**First action, regardless:** check whether `datos.energia.gob.ar` carries well-level production back to 2010 and through 2026, and email the guest editors to fix the deadline and sanity-check scope.
