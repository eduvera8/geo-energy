# Literature review — Paper 2


> **⚠️ SUPERSEDED IN PART — read `../NOVELTY-AUDIT-v2.md` first.** The novelty verdicts in this file came from a general-web scan. A domain-restricted scholarly screen (RePEc, NBER, SSRN, ScienceDirect, Wiley, IMF, World Bank) overturned two of them and found several references missing below.
# An implicit short option on oil: fuel-price smoothing rules and the fiscal cost of the 2026 disruption

**Status:** first draft of the review, 22 October 2026

---

## ⚠️ Citation reliability warning

Same constraint as Paper 1: **no PDF could be opened in this session.** WebFetch, curl and all direct HTTP are blocked; only a search tool works and it returns third-party summaries.

- **[S]** = existence and broad claim confirmed via search this session. Page numbers, coefficients and quotations are not verified.
- **[T]** = from training knowledge. The work probably exists as described, but year, journal, exact title or numbers may be wrong.

**Verify everything before it enters a bibliography.** See `PDF-REQUESTS.md` in the repository root.

---

## 1. The question

Latin America operates the world's densest collection of fuel-price smoothing mechanisms: Colombia's Fondo de Estabilización de Precios de los Combustibles (FEPC), Chile's Mecanismo de Estabilización de Precios de los Combustibles (MEPCO), Peru's Fondo de Estabilización, Ecuador's price bands, Bolivia's administered prices, Mexico's variable IEPS stimulus, and Brazil's discretionary Petrobras pricing policy. These are studied as subsidy policy, as pass-through frictions, or as fiscal-reform problems.

They are better understood as **derivatives**. Each rule defines a state-contingent transfer from the sovereign to fuel consumers as a function of the international product price. Each has an implicit strike (the rule-implied reference price), a notional (national fuel consumption), a maturity (the political horizon over which the rule holds), and — in every case — no hedge. A government operating a smoothing rule has written an uncovered short option on crude.

The 2026 disruption exercised those options simultaneously across the region, at a shock size no rule was calibrated for. That gives three questions:

1. **Pass-through:** how much of an international price change reaches the pump under each rule, and is the adjustment asymmetric?
2. **Tail behaviour:** do the rules *break* when the shock exceeds anything in their design range — that is, does pass-through jump non-linearly once fiscal capacity rather than the rule becomes the binding constraint?
3. **Valuation:** what was the option worth? What did the 2026 realisation cost each sovereign ex post, and what premium would have been fair ex ante at pre-war implied volatilities?

Question 3 is the novel core. Questions 1 and 2 are the econometric engine that makes 3 credible.

---

## 2. Strand A — Asymmetric pass-through ("rockets and feathers")

The methodological backbone. Large, mature, and mostly about OECD retail gasoline markets.

- **Bacon [T]**, "Rockets and Feathers: The Asymmetric Speed of Adjustment of UK Retail Gasoline Prices to Cost Changes," *Energy Economics* (approximately 1991). Names the phenomenon.
- **Borenstein, Cameron & Gilbert [T]**, "Do Gasoline Prices Respond Asymmetrically to Crude Oil Price Changes?", *QJE* (1997). The canonical asymmetric error-correction specification, and the one my Stage 1 adapts. **Essential — request PDF.**
- **Peltzman [T]**, "Prices Rise Faster Than They Fall," *JPE* (2000). Establishes the generality of the asymmetry across many markets, which matters because it means finding asymmetry in LatAm is *not* itself a contribution.
- **Deltas [T]**; **Lewis [T]** (search costs and asymmetry); **Verlinda [T]** (station-level, local market power); **Eckert [T]** (survey). The micro-mechanism literature: asymmetry arises from search frictions, inventory management and local market power.
- **Perdiguero / meta-analytic surveys [T]**. Useful for a sentence establishing the modal estimate against which LatAm regimes can be benchmarked.
- **Kilian & Zhou [T]**, on gasoline prices, oil prices and inflation expectations (*JAE*, approximately 2022), and related Kilian–Zhou work on oil prices and US inflation. **Directly relevant to the target issue's editorial interests and to my Stage 5 inflation counterfactual. Essential.**

**Positioning consequence.** Asymmetric retail pass-through is a crowded field and documenting it again in Latin America would be a weak paper. The contribution must be the *regime comparison*, the *tail breakdown*, and the *valuation* — not the asymmetry itself. Say this explicitly in the introduction so a referee does not mistake the paper for a replication.

## 3. Strand B — Latin American fuel pricing and the specific mechanisms

The strand where the novelty check did real damage, and where positioning matters most.

- **[S] "Retail Prices of Gasoline and Asymmetric Adjustment to Wholesale Prices in Colombia,"** *Journal of Economic Development* (2022). Indexed on RePEc/IDEAS; search returned only citation metadata, not findings. **Colombian asymmetric pass-through is therefore already published.** I need this PDF to know exactly what is claimed and on what sample.
- **[S] "Decomposition of Retail Gasoline Prices and the Sources of Market Power: Evidence for Colombia,"** Springer (2026). Monthly station data from four major Colombian cities, January 2017 – November 2019. Decomposes retail prices into wholesale cost pass-through, strategic complementarities and market power; its appendix documents the FEPC's export-parity price calculation, which is directly useful for my rule-parameter construction. **Essential — and paywalled, so I need it from you.**
- **[S] IMF Chile technical assistance report** (2023, IMF eLibrary): notes that since MEPCO began operating in its current form in **2014**, retail gasoline and diesel price changes have **deviated from changes in international oil prices**. States the fact but publishes no pass-through estimate. **So there is no MEPCO pass-through coefficient in the literature — that part of the gap is real.**
- **[S] WTO presentation, "Chile's Policy Response to the 2026 International Fuel [Price Shock]"** (Sebastián Gonzáles). Describes MEPCO as smoothing domestic prices of gasoline, diesel and vehicular LPG/CNG **by raising and lowering the specific fuel taxes**. This is the mechanical detail the option-strike construction needs, and it is a 2026 document, so it may describe the rule's behaviour during the shock. **High priority.**
- **[S] SEI, "A Strategic Phase-out of Colombia's Diesel Subsidy"** (2024). Reports the FEPC was established in **2007**, covers retail price disparities versus the international market, earns when national prices exceed international prices and spends when they fall below, and that the **2022 deficit reached 2.5% of GDP**. That number is the proof of concept for the entire paper: an option position large enough to matter macroeconomically. **Free PDF.**
- **[S] Latin American Energy Economics Meeting paper on FEPC institutional design** (9ELAEE): argues the FEPC has generated fiscal, economic and environmental problems that question its effectiveness and sustainability. Institutional critique, not estimation.
- **[S] ENAP estimated price reports** (Chile). Operational source for the weekly reference-price series — a data source more than a reference.
- **[S] Fedesarrollo, *Tendencia Económica* no. 226** (Colombia). Likely contains FEPC deficit analysis; worth checking.
- **[S] World Bank, "Global Landscape of Fuel Subsidies and Price Controls," April 2025.** Cross-country inventory of price-control mechanisms — the obvious source for classifying regimes consistently and for establishing that the LatAm sample is representative of a global phenomenon. **Essential, free.**

**What this strand lacks:** no comparative estimation across regimes on a common sample and benchmark; no tail/state-dependent estimation anywhere; no MEPCO pass-through estimate at all; and nothing on the 2026 episode.

## 4. Strand C — Fuel subsidies, fiscal cost and reform

Context for magnitude, and the literature the paper's policy contribution speaks to.

- **[S] IMF, "Underpriced and Overused: Fossil Fuel Subsidies Data 2025 Update"** (WP/2025/270). Distinguishes **explicit** subsidies (in budgets) from **implicit** ones (underpricing relative to environmental cost), and notes that fiscal gains from reforming implicit subsidies are smaller than the implicit subsidy itself because higher prices erode the fuel-tax base. **Important terminological warning: this literature's "implicit subsidy" means environmental underpricing, which is NOT what I mean by "implicit option." Define terms carefully or referees will conflate them.** Essential.
- **Coady, Parry et al. [T]**, the IMF energy-subsidy series. Standard reference for subsidy magnitudes and reform experience.
- **[S] World Bank, "Tracking Global Social Policy Responses to High Energy [Prices]."** Catalogues the 2021–23 policy responses; a useful comparison episode for the 2026 tail test.

## 5. Strand D — Contingent liabilities and fiscal risk

The strand the option framing plugs into — and the one where the gap is cleanest.

- **[S] Polackova, "Contingent Government Liabilities: A Hidden Risk for Fiscal Stability,"** World Bank Policy Research WP 1989, and the *Finance & Development* version (1999). The canonical fiscal-risk matrix: liabilities are **direct or contingent** × **explicit or implicit**. Fuel-price smoothing rules are explicit-contingent where codified in law (FEPC, MEPCO) and implicit-contingent where discretionary (Brazil). Use this taxonomy as the framing device.
- **[S] Cebotari, "Contingent Liabilities: Issues and Practice,"** IMF WP/08/245. Notes that **implicit contingent liabilities are by far the most costly** on available evidence. Directly supports the paper's motivation.
- **[S] World Bank WPS1989** also argues that off-budget support instruments (guarantees, insurance schemes) carry hidden costs relative to budgetary subsidies — the same argument this paper makes for price-smoothing rules.

**The confirmed gap.** A targeted search for option-pricing or contingent-claims valuation of fuel price caps **returned nothing**. The fiscal-risk literature stops at taxonomy and at scenario-based fiscal stress testing; it does not price these positions as derivatives. The energy-economics literature studies pass-through but not the fiscal position. **Nobody has valued a fuel-price smoothing rule as an option.** That is the paper's novel core, and it survived the check.

## 6. Strand E — Sovereign commodity hedging

The natural comparison: if the state is short an option, why not buy the offsetting one?

- **Mexico's sovereign oil hedge [T]** — the annual Hacienda put-option programme — is the standing real-world example of a government buying commodity options at scale, and the obvious benchmark for "what would hedging this position cost?" Documentation appears in SHCP budget documents. (This is also the hook of the separate Mexico proposal in `../EXTENDED-ABSTRACTS.md` §I.5; the two papers should cross-reference but not overlap.)
- **Daniel [T]**, IMF work on hedging commodity price risk in developing countries. **Borensztein & Panageas / Caballero [T]**, on commodity-linked sovereign debt instruments. **Verify these attributions carefully — this is a strand where my recall is weak.**
- **Devlin & Titman [T]**, on managing oil price risk in developing countries. Probably the closest existing treatment of the question "should a government hedge its fuel-subsidy exposure?"

**This strand needs your help.** It is where I am least confident and where the policy punchline lives: the ex-ante premium of the option the state wrote, compared against the cost of actually hedging it in the market.

## 7. Strand F — Threshold and nonlinear econometrics

Methods for the tail test.

- **Hansen [T]**, threshold regression inference (*Econometrica* approximately 1996 and 2000) — threshold estimation with bootstrapped p-values. **Essential for Stage 2.**
- **Granger & Teräsvirta [T]**; **van Dijk, Teräsvirta & Franses [T]** — smooth-transition models and their estimation. The STR alternative to a hard threshold.
- **Cameron, Gelbach & Miller [T]**, and **MacKinnon & Webb [T]** — wild cluster bootstrap with few clusters. **Non-negotiable for a panel of eight countries; cite it in the paper, not just in a footnote.**
- **Abadie et al. [T]** — synthetic control, for the Stage 5 inflation counterfactual.

---

## 8. The gap, stated precisely

1. **No comparative estimation across smoothing regimes.** Existing work is single-country (and for Colombia, already done). Nobody estimates pass-through across FEPC, MEPCO, IEPS and discretionary regimes on a common weekly sample against a common international product benchmark.
2. **No MEPCO pass-through estimate exists.** The IMF states that Chilean prices deviated from international prices post-2014 but quantifies nothing.
3. **No test of tail-state rule breakdown.** Every existing estimate is linear or at most sign-asymmetric. Whether a rule's pass-through regime *changes* once the shock exceeds its design range is unstudied, and 2026 is the first observation large enough to identify it alongside 2008, Libya 2011 and Russia 2022.
4. **No one has priced these rules as options.** Confirmed by targeted search. The fiscal-risk literature classifies them; the energy literature estimates pass-through through them; nobody values them.
5. **Nothing on the 2026 episode.**

**Contribution statement for the abstract:** we show that Latin American fuel-price smoothing rules are uncovered short option positions on crude, estimate their pass-through and tail breakdown on twenty-five years of weekly data across six to eight regimes, and value what the 2026 disruption cost each sovereign against the premium that would have been fair before the war.

---

## 9. Reading list priority

**Tier 1.** Borenstein, Cameron & Gilbert (1997); the two Colombian papers (JED 2022 and Springer 2026 — **both needed from you, the second is paywalled**); IMF Chile TA report (2023); Kilian & Zhou on gasoline and inflation; World Bank *Global Landscape of Fuel Subsidies and Price Controls* (2025); IMF WP/2025/270; Cebotari IMF WP/08/245; Polackova (1999); Hansen threshold papers; MacKinnon & Webb on wild cluster bootstrap.

**Tier 2.** Bacon (1991); Peltzman (2000); the WTO Chile 2026 presentation; SEI Colombia diesel paper; 9ELAEE FEPC paper; Fedesarrollo *Tendencia Económica* 226; World Bank energy-policy-response tracking; Devlin & Titman; Daniel on commodity hedging.

**Tier 3.** The station-level asymmetry micro literature (Lewis, Verlinda, Deltas); Abadie synthetic control; smooth-transition methodology.

---

## 10. Open questions for you

1. **Which countries do you want in the panel?** My default is Brazil, Chile, Colombia, Peru, Mexico, Uruguay — six with usable weekly or monthly price series and well-documented rules. Ecuador and Bolivia have the most dramatic policies but the worst data. Adding them raises the cluster count from 6 to 8, which matters for inference, but the data quality may not support them.
2. **Do you read Spanish regulatory documents comfortably?** Reconstructing MEPCO's and the FEPC's rule parameters means working through CNE and MinMinas resolutions. That work cannot be automated and I cannot access the documents from here.
3. **Is the option-valuation section something you want to carry, or should it be framed more conservatively as an accounting exercise?** The full Monte Carlo valuation with a jump component is the novel part but also the most attackable; a referee may regard it as over-engineering. My view is to carry it, lead with the sensitivity analysis, and keep the realised-cost accounting as the fallback headline.
4. Do you have, or can you get, **pre-war Brent option implied volatility surfaces** (late 2025 / early 2026)? The ex-ante premium calculation needs them. CME settlement vols may suffice.
