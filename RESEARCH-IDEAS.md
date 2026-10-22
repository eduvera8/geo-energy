# Research ideas for *Energy Economics* SI — "The Role of Geopolitics in Energy Markets"

**Prepared:** 22 October 2026 · **Revised:** 22 October 2026 (v2 — re-scored on econometric data adequacy)
**Target:** Elsevier *Energy Economics*, special issue 334954, guest editors **Lutz Kilian, Michael D. Plante, Siquan Wang**
**Constraint set:** Latin America preferred (not binding); econometrics must survive this editorial team; **feasibility means data adequate for estimation, not researcher time.**

---

## 0. Before anything else: verify the call

I could not open the ScienceDirect page from this environment (network policy returns 403 for `sciencedirect.com`), so the following is from search summaries and **must be confirmed on the journal page or by emailing the guest editors**:

| Item | What I found | Confidence |
|---|---|---|
| Journal | *Energy Economics* | High |
| Guest editors | Kilian, Plante, Wang | High |
| Scope | Geopolitical energy **supply disruptions**, explicit interest in the Iran War and the Hormuz closure (late Feb 2026, ~20% of global oil/LNG flows); editors want "questions and practical problems not commonly considered in the literature" | Medium-high |
| Deadline | **Conflicting**: 30 Jun 2026 (lapsed), 2 Nov 2026, 15 Jan 2027, 31 Jul 2027 across different Elsevier pages | **Low — resolve first** |

---

## 1. The editorial filter

**Rewarded:** physical-market realism (barrels, inventories, spare capacity, refinery runs, ton-miles, takeaway capacity); a *named and dated* shock with a visible first stage; parameters the literature is forced to assume (short-run supply elasticity above all); pass-through to fuel prices, inflation and inflation expectations; policy objects that actually exist (reserve releases, sanctions licences, smoothing funds).

**Penalised — near-automatic rejection risk:** a geopolitical-risk *index* on the right-hand side of a return regression; TVP-VAR "connectedness" and Diebold–Yilmaz spillover tables; wavelet coherence; quantile-on-quantile; NARDL for its own sake; GARCH volatility-spillover papers; "oil price" as a scalar shock with no supply/demand decomposition; daily-return event studies with no mechanism and no quantity evidence; loosely applied local projections (generated regressors, no lag augmentation, SEs ignoring first-stage estimation error).

Kilian's *Facts and Fiction in Oil Market Modeling* (*Energy Economics* 110, 2022) is the explicit statement of the standard he applies — read it as the referee report you will receive and pre-empt it in your identification section. Also: Kilian & Zhou on oil-market VAR econometrics, Känzig (2021, *AER*) for the oil-supply-news instrument, Baumeister–Hamilton for the counter-position.

---

## 2. The event landscape (your identification capital)

From reporting; re-verify each against a primary source before citing:

- **Iran War from 28 Feb 2026.** Hormuz effectively closed since. Brent spiked ~50% to near $120, then traded $80s–$112 through October on reopening rumours; reportedly still closed as of 22 Oct 2026.
- **Gulf producers cut output** because barrels were stranded behind the closure — a supply disruption that is simultaneously a landlocked-surplus event. Under-theorised.
- **IEA considered its largest-ever coordinated stock release.**
- **Venezuela, Dec 2025–Feb 2026:** regime change (sources conflict: S&P says removal ~Dec 2025; a trade outlet says capture early Jan 2026 plus a naval blockade), then sanctions easing, expanded Chevron authorisation, export licences for Vitol and Trafigura. Output to ~1.1–1.2 mb/d by mid-2026, a seven-year high. **A second, opposite-signed, LatAm geopolitical supply shock, dated weeks before the war.**
- **LatAm as residual supplier:** Rystad-sourced reporting puts South American government revenue ~$43bn above the pre-war baseline for 2026 (Petrobras ~$13.1bn); Brazil >3 mb/d with little headroom; Argentina a record ~887 kb/d.
- **LatAm as victim:** Chile, Peru, Central America and the Caribbean import nearly all fuel. **Mexico's refined-product import bill exceeded crude export earnings in early 2026, first time in ≥36 years.** Brazil sources ~40% of fertiliser through Hormuz.

**Critical feature for identification:** the Hormuz episode is **not one event**. It is a sequence of datable news shocks — the 28 Feb strikes, the March mixed messages and sub-$80 round trip, the IEA release, Iran's 10 Aug conditions, the US rejection of the reopening plan, the October swings. Plausibly 30–60 datable events over eight months. That matters enormously for what follows.

---

## 3. The real feasibility constraint: post-shock observations

**The correction to the premise.** LatAm customs data is not annual. Brazil's Comex Stat publishes HS8 × destination × port/state **monthly** with roughly a two-week lag, back to 1997; Mexico (INEGI) and Colombia (DANE) are monthly too; UN Comtrade carries monthly series. So the frequency is better than feared.

**But the objection stands anyway, and it is the right objection.** A February 2026 shock with a late-2026/2027 submission gives **about eight post-shock monthly observations**. That is fatal for any design where identification comes from time-series variation in an aggregate shock — and monthly trade data is exactly such a design.

**The point that does the work:** when the shock is *common to all units*, cross-sectional size does not substitute for time-series length. Adding thousands of wells or municipalities does not add independent information about an aggregate shock; the shock is collinear with the time effect. N buys precision on a common time effect, not identification. This is why "I have 3 million station-day observations" is not an answer to "you have eight months."

There are exactly three escapes, and every viable paper for this call uses at least one:

**Archetype A — Differential exposure.** Make the shock cross-sectionally varying: pre-determined exposure × post. Identification comes from comparing high- and low-exposure units, so eight months is ample (you have N × 8 and the interaction is identified). Requirements: an exposure measure fixed before the shock, parallel pre-trends, and exposure that is not itself a proxy for something else. Shift-share/DiD inference applies (Borusyak–Hull–Jaravel, Adão–Kolesár–Morales for shift-share SEs).

**Archetype B — Long-sample estimation, 2026 as out-of-sample.** Estimate the structural model or parameter on 1974–2025 (or a 2010–2025 panel with several price cycles), then use 2026 for conditional forecasting, historical decomposition, counterfactuals and out-of-sample validation. **2026 enters the paper as the motivating application, not the estimation sample.** This is Kilian's own practice with new events, and it dissolves the short-sample problem completely.

**Archetype C — High-frequency identification with many dated shocks.** Daily or intraday data, with the 30–60 datable war-news events of §2 as repeated realisations. Eight months is ~165 trading days and dozens of events — a usable narrative/high-frequency shock series. This is the only route by which the 2026 episode itself identifies anything.

**The ideal paper combines B and C for the price/market stage, and A for the real-outcome stage.** Long-sample structure for the parameter, high-frequency events for the shock, differential exposure for the transmission.

### What Latin America actually publishes above monthly frequency

| Frequency | Series | Confidence |
|---|---|---|
| Intraday/daily | Futures settlements (Brent, WTI, Mars, WCS, RBOB, HO; CME JKM futures as a free-ish LNG substitute); FX; sovereign spreads (ICE BofA via FRED); LatAm energy equities and ADRs (Petrobras, Ecopetrol, YPF, Vista, GeoPark) | High (CME JKM: verify) |
| Hourly | Brazil CCEE PLD (hourly since ~2021) and ONS dispatch, load, reservoir inflows; Argentina CAMMESA dispatch and costs; Chile Coordinador Eléctrico marginal cost; Colombia XM bolsa prices | High on existence, medium on exact vintages |
| Daily | Mexico CRE station-level fuel prices (~13k stations; reportedly degraded from 3×/day to 1×/day years ago) | Medium-high — verify first |
| Weekly | **Brazil ANP fuel-price survey by municipality/station, back to ~2001** — a ~25-year weekly panel, the single best LatAm energy price dataset; Chile CNE; Peru Osinergmin; EIA WPSR; Brazil Focus survey; Mexico IEPS stimulus in the *DOF* | High |
| Monthly | ANP production by field/well; Argentina Secretaría de Energía well-level production and fracture data; Comex Stat HS8 × destination × port; OPEC MOMR; industrial production; CPI; ANTAQ berth-level port calls (2010–present) | Medium-high — the Argentine and ANTAQ datasets I could not reach to verify |
| Paywalled | Kpler/Vortexa AIS tanker tracking; Argus/Platts assessments; JKM spot | — |

The weekly ANP series and the hourly power-system data are the two assets that make LatAm work on this shock econometrically viable. Build around them.

---

## 4. The long list, re-scored on data adequacy

**Data** = post-shock observations with independent shock variation, or a long estimation sample (weight 0.40); **Fit** = probability this editorial team wants it (0.35); **Novelty** = 0.25. Archetype column shows how each escapes the short-sample problem.

| # | Idea | Arch. | Data | Fit | Nov | Weighted |
|---|---|---|---|---|---|---|
| **4** | **Global gas shock × hydrology → electricity prices and industrial output (BR/AR/CL)** | A+B | 5 | 4 | 5 | **4.65** |
| **1** | **Short-run supply elasticity of LatAm oil, well-level (2010–2026), Hormuz as out-of-sample** | B+A | 5 | 5 | 5 | **5.00** |
| **3** | **Fuel-price stabilisation funds: 25-year weekly pass-through, 2026 as the tail test** | B+A | 5 | 5 | 4 | **4.75** |
| **19** | **Chokepoint-episode panel: Hormuz 2026, Red Sea 2024–25, Panama 2023–24, Suez 1956/1967/2021** | B+C | 5 | 4 | 5 | **4.65** |
| **2** | **Venezuela's reopening + the war: two opposite-signed supply shocks, state-dependent responses** | C+B | 4 | 5 | 5 | **4.60** |
| 6 | Fertiliser through Hormuz → Brazilian planting decisions (municipal shift-share) | A | 3 | 3 | 5 | 3.50 |
| 9 | Oil news and EM inflation expectations (weekly Focus, daily events) | C+B | 5 | 4 | 3 | 4.15 |
| 10 | Station-level rockets-and-feathers in Mexico under the war shock + IEPS offset | C+A | 4 | 4 | 3 | 3.75 |
| 5 | Mexico's flip from oil winner to oil loser (**redesigned** — see §5) | B | 3 | 4 | 4 | 3.60 |
| 7 | Hormuz × Panama Canal capacity (slot-auction clearing prices) | C | 4 | 4 | 5 | 4.25 |
| 8 | Ton-miles and destination reallocation of LatAm crude (monthly trade data) | A | 2 | 4 | 4 | 3.20 |
| 11 | Strategic reserves without an SPR: LAC days-of-cover, incidence of the IEA release | C+B | 3 | 4 | 4 | 3.60 |
| 12 | LAC sovereign spreads: who pays the geopolitical premium? | C | 5 | 3 | 2 | 3.55 |
| 13 | Distributional incidence across LAC households (microsimulation) | A | 3 | 3 | 4 | 3.25 |
| 14 | Diesel → freight tariffs → regional food CPI (Brazil) | A | 3 | 3 | 3 | 3.00 |
| 15–18 | Resource nationalism; Caribbean tariffs; Argentina LNG real options; lithium triangle | — | ≤3 | ≤3 | ≤4 | <3.0 |

**What the re-scoring changed.** Idea 5 (Mexico) falls from 2nd to 9th: its original form was a structural-break test with eight post-break observations, which has no power — I had it wrong, and §5 gives the repair. Idea 8 (ton-miles from trade data) falls out of contention for exactly your reason: monthly customs data gives eight points against an aggregate shock, and the destination-exposure variation is too coarse to rescue it. Ideas 4 and 19 rise, because hourly power data and a multi-episode panel are the two designs where sample length simply is not a constraint.

---

## 5. The five

### #1 — How elastic is Latin American oil supply? Well-level evidence, 2010–2026
**Top recommendation. Estimated on fifteen years; Hormuz is the out-of-sample application.**

**Question.** Oil-market SVARs must take a stand on the short-run price elasticity of supply, and the Kilian–Murphy vs. Baumeister–Hamilton debate turns on it. Credible micro estimates exist essentially only for US shale. Nobody has estimated it for Vaca Muerta or Brazilian pre-salt — which in 2026 is precisely where the marginal non-OPEC barrel was supposed to come from. You deliver a parameter the literature is forced to assume.

**How the short sample is handled.** Estimation uses the **2010–2025 well-level panel**, which contains the 2014–16 collapse, the 2020 COVID collapse and the 2021–22 spike — ample price variation and ~180 months. **2026 is then (i) an out-of-sample test of the fitted elasticity, and (ii) the test of a state-dependent prediction:** the response should be smaller than history implies, because takeaway capacity binds. That is a falsifiable out-of-sample claim, which is a much stronger paper than an eight-month regression.

**Data.** Argentina: Secretaría de Energía open data — monthly well-level production plus the fracture/completion dataset (stage counts, lateral length, proppant). Brazil: ANP monthly production by field and well, plus drilling and concession data. Colombia: ANH/Ecopetrol field-level. Guyana: no granular data — aggregate case study, not a panel unit. **Verify the Argentine datasets in week 1; `datos.energia.gob.ar` was unreachable from here.**

**Specification.** Two margins, separately — the distinction matters because aggregate studies conflate them.
1. *Extensive (drilling/completions),* operator × basin × month, local projections with lag augmentation:
   $y_{i,t+h} - y_{i,t-1} = \alpha_i^h + \beta^h \varepsilon_t^{oil} + \gamma^h(L) X_{i,t-1} + u_{i,t+h}$, $h=0,\dots,18$, with $\varepsilon^{oil}$ a Känzig-style oil supply news shock. Two-way clustering; Driscoll–Kraay for cross-sectional dependence; bootstrap the first-stage estimation error into the bands.
2. *Intensive (existing wells).* Fit pre-shock type curves by vintage cohort and formation; test post-shock deviations from predicted decline (choke management, workovers, refracs).

**Mechanism (Archetype A, and what makes it a paper rather than a regression).** Interact with **takeaway capacity** (Oldelval / Vaca Muerta Sur utilisation), operator liquidity and foreign ownership, and Argentina's policy regime (RIGI, FX unification). The elasticity is a capacity-constrained object with a shadow price you can estimate — which is the direct answer to "can the Western Hemisphere replace Hormuz barrels, and how fast?"

**Close** with a table comparing your estimate to the priors imposed in the existing SVAR literature, and what they imply for the price response to a chokepoint closure.

**Residual risks.** Argentine policy changes confound the 2026 window (use Brazil as the policy-stable comparison); pre-trends from the 2025 ramp-up (cohort FE, explicit pre-trend tests); dataset access.

---

### #4 — Qatari LNG, hydrology, and the price of electricity (Brazil, Argentina, Chile)
**Best data position on the list. Hourly outcomes, continuously varying exposure, long sample.**

**Question.** Hormuz carried roughly a fifth of global LNG. South American power systems are hydro-dominated with gas and diesel at the margin, so the same global gas shock hits hard or barely at all depending on the hydrological state — which is plausibly exogenous and varies continuously. That interaction identifies the pass-through of a geopolitical gas shock into spot power prices, thermal dispatch, and ultimately industrial output.

**Why the sample problem never arises.** The outcome is hourly and the exposure varies day to day, so the eight post-shock months are tens of thousands of observations with *genuine within-period variation in treatment intensity* — not one aggregate shock. The long sample (Brazil PLD from ~2001, hourly from ~2021) supplies additional gas-price cycles (2021–22 especially) for Archetype B validation.

**Design.** Plant/system level, daily or hourly:
$y_{p,t} = \beta_1 \varepsilon^{gas}_t + \beta_2 H_t + \beta_3(\varepsilon^{gas}_t \times H_t) + \alpha_p + \delta_{week} + \Gamma' X_{p,t} + u_{p,t}$
with $H_t$ reservoir inflow/storage relative to its historical distribution. $\beta_3$ is the object of interest. Second stage on real outcomes: electricity-intensity shift-share across manufacturing sectors (monthly sectoral industrial production) and the CPI electricity component.

**Data.** Brazil: ONS (natural energy inflows, reservoir levels, dispatch), CCEE PLD, ANEEL tariff flags. Argentina: CAMMESA, plus **ENARSA LNG tender awards (public award prices — a genuinely useful free substitute for JKM)**. Chile: Coordinador Eléctrico marginal costs and dispatch, GNL Quintero. Gas-price shock: CME JKM futures settlements and/or TTF, Henry Hub from EIA, cross-checked against tender awards. **Settle this series in week 1** — JKM spot assessments are paywalled and the measurement choice is attackable.

**Risks.** Hydrology and global gas prices may correlate through global weather (control for ENSO indices and test explicitly). Regulated tariffs mute consumer pass-through — measure that as a result, which links directly to #3's contingent-liability story.

---

### #3 — Who pays for smoothing? Stabilisation funds under a tail geopolitical shock
**Safest high-fit option. Twenty-five years of weekly data; 2026 is the stress test.**

**Question.** Latin America is the densest laboratory of fuel-price smoothing rules in the world: Colombia's FEPC, Chile's MEPCO, Peru's FEPC, Ecuador's bands, Bolivia's fixed prices, Mexico's variable IEPS stimulus, Brazil's discretionary Petrobras policy. None was stress-tested against a disruption of this size. Three results: (i) pass-through of international *product* prices to the pump by regime, including asymmetry; (ii) the **contingent fiscal liability** these rules created — an implicit short option on oil that these states wrote and the war exercised; (iii) counterfactual CPI paths had each country used its neighbour's rule.

**How the short sample is handled.** Pass-through parameters are estimated on the **long weekly panel (~2001–2025)**, which contains 2008, Libya 2011, the 2014–16 collapse, 2020 and Russia 2022 — many shocks, hundreds of weeks, several regime changes. 2026 is then the out-of-sample tail test: *do the estimated rules still describe behaviour when the shock exceeds the 99th percentile of the historical distribution?* Where they break, that break is the finding.

**Data.** Brazil ANP weekly survey (municipality/station level, ~2001–present); Chile CNE weekly; Colombia MinMinas/Ecopetrol; Peru Osinergmin *Facilito*; Mexico CRE plus weekly IEPS rates in the *DOF*; Uruguay URSEA/ANCAP. Benchmarks: **USGC conventional gasoline and ULSD spot from EIA (free)** — use product, not crude, or a referee will correctly object. Fiscal cost from budget execution and FEPC/MEPCO statements; CPI weights from national statistics offices.

**Specification.** Borenstein–Cameron–Gilbert-style ECM with regime interactions:
$\Delta p^{ret}_{c,t} = \sum_j(\theta_j^+\Delta x^+_{c,t-j} + \theta_j^-\Delta x^-_{c,t-j}) + \lambda(p^{ret}_{c,t-1} - \mu_c - \nu_c x_{c,t-1}) + \delta'(\text{regime}_c \times \Delta x_{c,t}) + \text{FE} + \epsilon_{c,t}$
plus a threshold version (shock above the historical 95th/99th percentile) to test rule breakdown under tail shocks; then the fiscal-liability calculation (realised wedge × volumes) and synthetic-control inflation counterfactuals across regimes.

**Inference discipline — raise it before the referee does.** Eight countries is few clusters: wild cluster bootstrap, and consider the station-level Brazilian panel as the high-powered within-country complement. Date every 2026 rule change narratively; several countries altered their rules mid-year, which is a feature if dated and fatal if ignored. Brazil's policy is discretionary, not a rule — separate category.

---

### #19 — What happens when a chokepoint closes? Evidence from six episodes
**New idea, added in this revision. The design in which sample length is structurally a non-issue.**

**Question.** The literature treats chokepoint risk as a scenario exercise, not an estimated object. Build the first econometric panel of **chokepoint capacity-loss episodes**: Hormuz 2026, Bab el-Mandeb/Red Sea 2024–25, the Panama Canal drought restrictions 2023–24, Ever Given 2021, the Hormuz tanker war 1984–88, and the 1956 and 1967 Suez closures. Estimate the response of crude and product prices, freight rates, ton-miles, insurance premia and destination reallocation to a unit of lost chokepoint throughput — then ask what the estimated elasticity implies for 2026, and how much of the adjustment the Western Hemisphere absorbed.

**Why it solves your problem.** Identification comes from **variation across episodes**, not from eight months of one episode. Each episode contributes daily data over months, with measurable treatment intensity (throughput lost, ton-mile increase, duration, anticipation). 2026 is the largest observation in the panel, which is exactly the role a new event should play.

**Data.** Baltic Dirty/Clean Tanker indices and route-specific rates; Suez Canal Authority and Panama Canal Authority transit counts — **and the Panama Canal's slot-auction clearing prices, a market-priced measure of chokepoint scarcity that the energy literature has essentially never used**; EIA prices and flows; historical episodes from archival sources and the shipping literature. Latin American content: differentials and destination mix for Brazilian, Guyanese, Colombian and Mexican crude as the residual-supplier margin.

**Fit.** Directly on the call's language — a practical problem not commonly considered, with physical quantities throughout, and a reusable parameter. Risk: assembling the historical episodes is genuine archival work, and pre-1970 price data is thin, so the panel may reduce to four usable episodes.

---

### #2 — Two geopolitical supply shocks, six weeks apart: Venezuela's reopening and the Hormuz closure
**Highest novelty. First-mover on the 2026 Venezuelan reopening.**

**Question.** Within six weeks world oil supply received a *positive* geopolitically-driven shock (Venezuelan sanctions relief, ~+0.5 mb/d, dated Jan–Feb 2026) and a *negative* one roughly thirty times larger. Is the price response per barrel symmetric? Theory says no: with inventories drawn and spare capacity stranded behind a closed strait, the response per lost barrel should be far larger in the war state. You estimate that state dependence from two cleanly dated, opposite-signed, *geopolitical* shocks — a structural asymmetry, not a GARCH one.

**How the short sample is handled.** The event study is Archetype C: daily (intraday if obtainable) windows around OFAC/Treasury licence actions and the 30–60 war-news dates of §2 — dozens of events, not two. The state-dependence parameter is estimated on a long-sample structural oil-market VAR (Archetype B) with inventory cover / OECD days-of-supply as the state variable, and 2026 enters via historical decomposition and counterfactual paths.

**Quantities, which is what sells it.** Heavy-sour differentials (Maya formula price, WCS–WTI, Mars–WTI from CME settlements); **EIA weekly US crude imports by origin**; **PADD 3 refinery crude inputs and utilisation**; USGC crack spreads; Venezuelan output from OPEC MOMR secondary sources cross-checked against Chevron's 10-Q disclosures; synthetic control for the output recovery itself.

**Risks — the weakest data position of the five.** Venezuelan quantity data is genuinely poor: use bounds, not point estimates, and say so. Political reversal risk during review. The Jan–Feb window is clean of the war, which is the design's main asset — protect it by dating events precisely.

---

## 6. The repair to idea #5, and why I am demoting it

**Mexico's flip from oil winner to oil loser** was my second recommendation in v1. As specified — structural break tests (Andrews QLR, Bai–Perron) on the oil beta of the peso and sovereign spreads — it fails your criterion and I was wrong to rank it there. Eight post-break monthly observations cannot identify a break; the tests have essentially no power and a referee will say so in one line.

**The repair, which makes it publishable again:** stop treating the flip as a *break* and treat it as a *state*. Mexico's net oil position moved continuously for three decades — exports declining since 2004, product imports rising throughout — so estimate a **state-dependent model over 1993–2026 in which the state is the continuously measured net oil position** (or net oil revenue as a share of exports/fiscal revenue). You then have thirty years of variation in the state variable, the coefficient of interest is identified off the whole sample, and 2026 is the extreme realisation that tests the fitted state dependence out of sample. Same economics, same headline, actual identification.

The **sovereign hedge** component survives untouched and is the most original part: the Hacienda buys crude puts annually, and 2026 is the realisation in which the hedge paid off on an exposure Mexico arguably no longer runs. Value the programme against the realised path (daily CME options data, SHCP-published strikes/volumes/premia) and ask whether a product-import hedge now dominates a crude-export put. That is a real policy question nobody has asked.

Even repaired it ranks fifth or sixth, because the identification rests on a state variable that moves slowly and correlates with everything else about Mexico's economy over thirty years. Take it if you want the macro-finance paper; otherwise #19 is the better fifth slot.

---

## 7. Also worth a look

- **#9 Oil news and EM inflation expectations.** Weekly Focus survey plus the daily war-news event set; a direct extension of Kilian–Zhou to emerging markets under a tail shock. Low novelty, excellent data, and it shares the entire data build with #3.
- **#7 Hormuz × Panama.** Can stand alone on the slot-auction price data, or fold into #19 as one episode. Folding is better.
- **#6 Fertiliser through Hormuz.** The most "not commonly considered" idea I have, and clean Archetype A (municipal crop mix × fertiliser intensity × Hormuz-origin exposure). Held back only because the planting response is observed annually and the 2026/27 season is just beginning. If the deadline is Jul 2027, promote it.
- **#12 LAC sovereign spreads.** Daily data, trivially feasible, but the literature is crowded and the fit is mediocre. Only as a section of another paper.

---

## 8. Recommendation

**First choice: #1.** Fifteen years of well-level data for estimation, 2026 as a falsifiable out-of-sample test, a parameter the editors' own literature cannot settle, and Latin America because that is where the marginal barrel actually is. The data constraint you raised does not bind on it once estimation moves to history.

**If you want the cleanest identification: #4.** Hourly outcomes and continuously varying exogenous exposure; the short-sample problem never arises.

**If the deadline is weeks away: #3.** Twenty-five years of weekly prices already in a usable form, and the tail-test framing turns the recency of the shock from a liability into the research question.

**Best pairing:** #3 first — it builds the regional weekly price database — then #1 as the follow-up. #19 if you want the highest-ceiling paper and are willing to do archival work. #2 if you want the first-mover claim on Venezuela and can tolerate the worst data of the five.

**The general principle for this call:** use 2026 as the motivation, the application and the out-of-sample test — never as the estimation sample.

---

## 9. Week-1 data verification (before writing a word)

1. Email the guest editors: operative deadline + scope check on your top pick.
2. **Argentina:** confirm `datos.energia.gob.ar` well-level production and fracture datasets — existence, coverage back to 2010, whether 2026 months are posted. Unreachable from this environment; this single check decides whether #1 is viable.
3. **Brazil:** confirm ANP well/field monthly production through Q3 2026, and pull the ANP weekly fuel survey history to check how far back station/municipality detail actually goes (the ~2001 start is my recollection, not verified).
4. **Power systems:** confirm CCEE hourly PLD history and ONS inflow series; CAMMESA and Coordinador equivalents.
5. **Gas prices:** settle the LNG series for #4 — institutional access to JKM, else CME JKM futures settlements plus ENARSA tender awards.
6. **Mexico:** confirm CRE station-level price frequency and whether a full history is downloadable.
7. **Differentials:** check access to Maya/WCS/Mars realised prices for #2 (CME settlements free; Argus/Platts assessments are not).
8. **Chokepoints (#19):** confirm Panama Canal slot-auction clearing prices and Suez/Panama transit series are downloadable at daily or weekly frequency.
9. Build the 2026 narrative chronology now, with primary-source citations (OFAC notices, IEA statements, OPEC MOMR, national regulators), and **date the 30–60 war-news events** — the high-frequency identification in #2 and #19 lives or dies on it.

## 10. Referee-proofing checklist

- Name the shock, date it, show the first stage.
- Decompose oil prices; never regress on a scalar oil price or a GPR index.
- Report quantities alongside prices.
- State where identification comes from — exposure variation, long sample, or high-frequency events — in the first paragraph of the empirics. For this issue, pre-empt the obvious "you only have eight months" objection explicitly.
- Lag-augment local projections; bootstrap instrument-generated-regressor uncertainty into the bands; state clustering and use a wild cluster bootstrap with few clusters; use shift-share-appropriate SEs where exposure identifies.
- Pre-trends and placebos (the Jan 2026 Venezuela window as a placebo for war-shock specifications, and vice versa).
- Compare your estimate to the priors imposed in the existing SVAR literature, in a table.
- Address Kilian (2022) head-on in the identification section.
