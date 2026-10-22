# Literature review — Paper 1


> **⚠️ SUPERSEDED IN PART — read `../NOVELTY-AUDIT-v2.md` first.** The novelty verdicts in this file came from a general-web scan. A domain-restricted scholarly screen (RePEc, NBER, SSRN, ScienceDirect, Wiley, IMF, World Bank) overturned two of them and found several references missing below.
# Why offshore oil supply cannot respond: capacity-constrained elasticity and the allocation margin in Brazil

**Status:** first draft of the review, 22 October 2026
**Working title alternatives:** "Four Million Barrels and No Spare Capacity"; "The Capacity-Constrained Elasticity of Offshore Oil Supply"

---

## ⚠️ Citation reliability warning — read before using any reference below

**I could not open a single PDF in this session.** WebFetch, curl and every direct HTTP request are blocked in this container; only a search tool works, and it returns third-party summaries. Consequently:

- References marked **[S]** were confirmed to exist in this session via search, usually with a one-line finding. The existence, authorship and broad claim are reliable; exact page numbers, coefficients and quotations are **not**.
- References marked **[T]** come from my training knowledge. The paper almost certainly exists and the characterisation is probably right, but **the year, journal, exact title or specific numbers may be wrong.** Several are classics I am confident about; others are not.
- **Nothing here is safe to paste into a manuscript bibliography without verification.** Treat this document as a reading list and an argument map, not as a citation source.

`PDF-REQUESTS.md` in the repository root lists what I need from you, in priority order.

---

## 1. The question and why it is open

The short-run price elasticity of oil supply is the single most consequential free parameter in oil-market macroeconomics. It determines how much a given supply disruption moves price, which in turn determines the entire macro response. Every structural oil-market VAR imposes a value or a prior on it; every scenario exercise of the 2026 Hormuz closure embeds one implicitly.

The empirical basis for the values in use is remarkably thin and remarkably American. Credible well-level estimates exist for North Dakota and Texas. Nothing comparable exists for any producer outside the United States. The global short-run elasticity figure in common use (around 0.06–0.07) is not estimated globally; it is **constructed** by assuming US shale is the only price-responsive segment of world supply and scaling by its share. That assumption has never been tested against non-US microdata.

Brazil is the natural place to test it. At over 4 mb/d it is the largest non-OPEC producer in the Western Hemisphere after the United States, it was widely expected to be part of the answer to the 2026 disruption, and its production is almost entirely offshore pre-salt — a technology with a capital cycle measured in years rather than months. If the US shale elasticity does not transfer, the global parameter in use is wrong in a direction and magnitude that Brazilian microdata can establish.

**The paper's thesis:** Brazilian offshore supply has a short-run production elasticity near zero, bounded above by floating-production-unit processing capacity, and the margin that *does* respond within months is not production but **allocation** — the split of crude between export and domestic refining. For the question "could the Western Hemisphere supply more barrels to the world market in 2026?", the allocation elasticity is the relevant one, and nobody has estimated it.

---

## 2. Strand A — Micro-level estimates of oil supply elasticity

This is the strand the paper joins and the one it extends geographically.

- **Anderson, Kellogg & Salant [T]**, "Hotelling Under Pressure," *JPE* (I believe 2018). The foundational result for conventional wells: output from existing wells does **not** respond to price, because flow is constrained by reservoir pressure. Firms respond on the drilling margin instead. Establishes that the intensive and extensive margins must be analysed separately — the methodological point this paper inherits. **Essential reading; request PDF.**
- **Bjørnland, Nordvik & Rohrer [S]**, "Supply Flexibility in the Shale Patch: Evidence from North Dakota." Well-level data on 16,000+ wells. Finds shale well supply elasticity positive and in the range **0.3–0.9**, with **no comparable response from conventional wells**. This is the headline number the Brazilian estimate will be compared against. (Published in *Journal of Applied Econometrics*, I believe — verify.) **Essential.**
- **Aastveit, Bjørnland et al. [S]**, "The Price Responsiveness of Shale Producers: Evidence from Micro Data," *Quantitative Economics* (2026). Finds **both** margins respond significantly to price, with responsiveness notably **stronger for refracturing than for new completions**. This is the current frontier and directly shapes my Stage 2 design: the intensive margin is not uniformly dead, it depends on the available intervention technology. *Quantitative Economics* is open access, so this one should be easy to obtain. **Essential.**
- **Newell & Prest [T]**, "The Unconventional Oil Supply Boom: Aggregate Price Response from Microdata," *Energy Journal* (approximately 2019). Aggregates micro drilling responses into a supply elasticity; the methodological template for my Stage 3 aggregation. **Essential.**
- **Kellogg [T]**, "The Effect of Uncertainty on Investment: Evidence from Texas Oil Drilling," *AER* (around 2014). Drilling responds to volatility, not just level — relevant because 2026 was a volatility shock as much as a level shock, and a referee will ask whether my shock measure conflates them. **High priority.**
- **Smith & Lee [T]**, Decker/Covert-type work on shale productivity and learning. Needed to control for technological drift in type curves. Lower priority.
- **Commentary [S]:** a September 2026 piece disputes a spring-2026 aggregate elasticity estimate on the ground that drilled-but-uncompleted well inventory in March 2026 was too small to support it. Useful as evidence that the parameter is contested in real time, and it makes the same capacity-constraint argument this paper formalises — in the US context, for DUCs rather than FPSOs.

**What this strand lacks:** every estimate is onshore US, and all but Anderson–Kellogg–Salant are shale. There is no offshore estimate, no non-US estimate, and no treatment of processing-capacity constraints as the binding margin.

## 3. Strand B — The elasticity inside structural oil-market models

The strand that determines whether the editors care.

- **Kilian & Murphy [T]**, "The Role of Inventories and Speculative Trading in the Global Market for Crude Oil," *JAE* (2014). Imposes bounds on the short-run supply elasticity as an identifying restriction. The value imposed here is one of the two numbers the paper should speak to directly.
- **Baumeister & Hamilton [T]**, "Structural Interpretation of Vector Autoregressions with Incomplete Identification," *AER* (2019), and the oil-market application. Argues for Bayesian priors over the elasticity rather than hard bounds, and reaches different conclusions. The other number to speak to.
- **Kilian [S]**, "Facts and Fiction in Oil Market Modeling," *Energy Economics* 110 (2022). Responds to the Baumeister–Hamilton critique, argues parts of the econometric analysis attributed to Kilian & Murphy are mischaracterised, and draws **methodological lessons for applied researchers using structural VARs**. Written by a guest editor of the target issue; the identification section must engage it explicitly. Working-paper versions circulated as CEPR DP14047 and Dallas Fed WP 1907 and as CESifo WP 7902. **Essential — and I could not open any version, so I am reasoning about its content from secondary description only.**
- **Känzig [T]**, "The Macroeconomic Effects of Oil Supply News: Evidence from OPEC Announcements," *AER* (2021). The external-instrument approach I plan to adapt for the shock series. **Essential.**
- **Caldara, Cavallo & Iacoviello [T]**, "Oil Price Elasticities and Oil Price Fluctuations," *JME* (around 2019). Country-level supply-shock construction and elasticity estimation; the closest existing work to a non-US elasticity, but at country-aggregate rather than well level. **High priority — this is my nearest competitor and I need to position precisely against it.**
- **Kilian & Zhou [T]**, work on the econometrics of oil-market VAR models (*Advances in Econometrics*, approximately 2023). Methodological reference.

**What this strand lacks:** it needs the parameter and cannot produce it from aggregate data. That is the opening.

## 4. Strand C — Offshore development, real options and capacity constraints

The strand that supplies the paper's mechanism.

- **Dixit & Pindyck [T]**, *Investment Under Uncertainty* (1994). The option-value logic for why a 4–7 year offshore development cycle is nearly unresponsive to a transient price spike. Theory framing, not an empirical reference.
- **Enverus industry data [S]:** combined pre-salt FPSO takeaway capacity reported at approximately **1.35 mb/d**, with Petrobras planning roughly **$40bn of pre-salt spending over five years including 12 new FPSOs**. **Caution: the 1.35 mb/d figure is inconsistent with Petrobras-operated pre-salt output of ~3.88 mb/boe/d and probably refers to a subset of units or a specific hub. Do not use without verification** — but it signals that unit-level nameplate capacity data is assembled commercially and may be reconstructible from public sources.
- **EPE, *Brazilian Oil & Gas Report* series [S]** (2018/19 through 2024/25, published in English). Two useful descriptive findings: well breakeven costs fell approximately **40% between 2010 and 2017**, with investment continuing even under low-price scenarios; and **reduced investment in Campos Basin mature fields accelerated their decline as Petrobras reallocated capital to pre-salt**. The second is important — it is capital *reallocation*, not aggregate capex response, which means a naive price-on-output regression will understate the mechanism. **High priority for institutional background; free PDFs on EPE's site.**
- **Petrobras pre-salt disclosures [S]:** 2025 pre-salt output of 2.56 mboe/d own production and 3.88 mboe/d operated; national output first passed 4 mb/d in December 2025 (press report, verify against ANP).

**What this strand lacks — and this is the core finding of the novelty check:** **no econometric study estimates the price elasticity of Brazilian pre-salt output or of Petrobras investment.** Searching specifically for it returned only operational data, industry analytics and EPE's descriptive planning reports. The gap is clean.

## 5. Strand D — State ownership and national oil company investment behaviour

The strand that supplies the paper's main confound.

Brazil's upstream is dominated by one state-controlled operator. Petrobras capex responds to leverage targets, dividend policy, government ownership objectives and the electoral cycle, not only to price. The paper's extensive-margin identification must handle this, and a referee will raise it immediately.

- **Hartley & Medlock [T]**, on NOC objective functions and their deviation from profit maximisation. Needed to motivate the control strategy.
- **Victor, Hults & Thurber [T]**, *Oil and Governance* (around 2012), on NOC behaviour. Background.
- Literature on **Petrobras fuel pricing and political interference [T]** — there is a real body of work on the domestic fuel-price policy of the 2011–2014 period and the subsequent PPI/market-parity policies. Relevant here mainly because it bears on the *downstream* allocation margin, which is central to Paper 1's second contribution and which is also the subject of Paper 2. **I need help identifying the best references in this area — this is the strand where my knowledge is weakest and most likely to be out of date.**

**Mitigation to develop:** exploit within-Brazil variation across operators (the non-Petrobras share: Shell, Equinor, TotalEnergies, Petrogal, PetroRio/Prio, Karoon) and across fields under different contract regimes (concession vs. production-sharing vs. transfer-of-rights). If private operators respond and Petrobras does not, that is a result rather than a nuisance — and it identifies the political-economy channel cleanly.

## 6. Strand E — The 2026 disruption

- **Dallas Fed WP 2609 [S]** (April 2026): complete Hormuz closure removing close to 20% of global oil supply, no pipeline diversion to the Red Sea in the baseline; quarterly WTI rising from about $60 pre-war to about $103, falling to about $71 on reopening after one quarter.
- **Dallas Fed WP 2615 [S]** (June 2026): a 15% net world supply decline after diversion, benchmarked against a 5% shock described as the average of four historical disruptions; rest-of-world real GDP growth falls roughly six times as much as the US response.
- **Dallas Fed public analysis [S]** (March 2026): Q2 closure cutting global real GDP growth by approximately 2.9pp annualised, WTI averaging approximately $98.
- **Oxford Energy Forum 149 [S]** (May 2026): net shock of approximately 1.2 billion barrels in 2026, described as the largest oil shock in history.
- **World Bank Commodity Markets Outlook 2026 [S]:** largest oil market shock on record; projected 6.9 mb/d year-on-year decline in 2026 Q2 output.
- **Wikipedia, "2026 Iran war fuel crisis" [S]:** useful only as a chronology scaffold for the event dating, never as a citation.

**Strategic reading.** The 15% versus 5% benchmarking in WP 2615 is an implicitly **linear** scaling of supply shocks into outcomes, and all of these exercises must assume how much non-OPEC supply responds. **A guest editor is a Dallas Fed economist.** The paper should therefore position as supplying a parameter these models need, never as a competing estimate of the closure's aggregate effects. Make that explicit in the introduction and the cover letter.

---

## 7. The gap, stated precisely

1. **No non-US well-level supply elasticity exists.** The literature's elasticity estimates are North Dakota and Texas; the global parameter is an extrapolation from them.
2. **No offshore estimate exists at all**, onshore or off, US or otherwise. Offshore is roughly a quarter of world production.
3. **Processing capacity has never been treated as the binding constraint on the elasticity.** The US literature's analogue is DUC inventory; the offshore analogue — FPSO nameplate — is lumpy, unit-level, observable and dateable, which makes it a better-identified constraint than anything available onshore.
4. **The allocation margin is unstudied.** Whether a producing country's barrels reach the world market during a disruption depends on the export-versus-domestic-refining split, not on wellhead output. For an issue about a supply disruption, this is the economically relevant elasticity, and I found no estimate of it for any country.

**Contribution statement to use in the abstract:** we provide the first well-level estimates of the short-run price elasticity of offshore oil supply, show that it is bounded by processing capacity rather than by geology or finance, and identify the allocation margin as the only short-run channel through which a large offshore producer can supply additional barrels to the world market — then quantify how much that channel delivered during the largest supply disruption on record.

---

## 8. On dropping Argentina — the honest econometric assessment

**Brazil alone works, but it is a different paper, and the reframing above is what makes it work.**

What is lost without Argentina:
- Argentina is the only non-US unconventional play at scale. Since shale is the only segment of world supply with a demonstrated positive short-run elasticity, dropping it means the paper **cannot deliver a positive elasticity estimate** and cannot speak to whether the US shale number transfers. The headline becomes "offshore supply does not respond," which is closer to replicating Anderson–Kellogg–Salant in a new setting than to breaking new ground on the parameter.
- The shale-versus-deepwater contrast is what would have made the capacity-constraint mechanism general rather than Brazil-specific.
- Policy and institutional variation (administered prices, export duties, FX regimes, many competing private operators) is lost, and with it a useful robustness dimension.

What is gained:
- **Clean prices.** Brazilian producers face market-linked netbacks, so the netback-construction problem — administered domestic prices, export duties, FX gaps — disappears entirely. That was the single largest measurement risk in the two-country design.
- **A better capacity instrument.** FPSO nameplate capacity with staggered commissioning dates is unit-level and quasi-experimental, which is stronger than basin-level pipeline capacity.
- **Direct policy relevance.** Brazil at 4+ mb/d *is* the Western Hemisphere's non-US margin in volume terms, so the Hormuz-replacement question is literally about Brazil.

The real cost is not Argentina's size. It is that the paper loses the only comparison that would show the mechanism generalises. **My recommendation: build the Brazilian paper as the core — which is what the data plan does — and keep Argentina as a one-section extension that can be bolted on if the data check succeeds, framed as "the only non-US shale laboratory" rather than as a second country.** The marginal cost is low because the pipeline is the same, and the marginal return is high because a referee asking "does this generalise beyond deepwater?" has an answer. If you would rather not, the Brazil-only paper stands on its own with the reframe.

**One substantive warning about Brazil-only, which the design must address.** Brazil has many wells but few *decision units*: a handful of operators, dominated by one state-controlled firm, making lumpy multi-year capital commitments. The effective N on the extensive margin is small, and investment is driven by capex plans and politics as much as by spot price. That is the same N-versus-T problem in another guise. The design handles it three ways: (i) the intensive and allocation margins have genuinely large effective N and short decision lags; (ii) operator heterogeneity (Petrobras vs. private) turns the confound into an estimable channel; (iii) the long 2000–2025 estimation sample supplies the time-series variation the cross-section cannot.

---

## 9. Reading list priority

**Tier 1 — cannot write the paper without these.** Aastveit et al. (QE 2026); Bjørnland, Nordvik & Rohrer; Anderson, Kellogg & Salant; Newell & Prest; Kilian (2022, *EE*); Kilian & Murphy (2014); Baumeister & Hamilton (2019); Känzig (2021); Caldara, Cavallo & Iacoviello; Dallas Fed WP 2609 and WP 2615.

**Tier 2 — needed for the mechanism and the confound.** Kellogg (2014); EPE *Brazilian Oil & Gas Report* 2021/22 through 2024/25; ANP data dictionaries for the production datasets; NOC investment-behaviour references; Petrobras *Plano Estratégico* documents 2010–2026.

**Tier 3 — robustness and framing.** Decline-curve and type-curve methodology references; Hotelling and real-options theory; the Oxford Energy Forum 149 issue; World Bank *Commodity Markets Outlook* 2026.

---

## 10. Open questions for you

1. Do you have institutional access to Argus or Platts Brazilian crude assessments (Tupi, Búzios, Sapinhoá differentials to Brent)? If not, the data plan's workaround is a realised export price built from Comex Stat value-over-volume, which is defensible but coarser.
2. Do you know whether ANP's well-level production data identifies the **production unit** (FPSO/platform) each well flows to? The entire capacity-constraint design depends on that linkage. If it does not, we need to build the well-to-unit crosswalk by hand from field development plans.
3. Is there a Brazilian literature on Petrobras investment behaviour I should know about, in Portuguese, that would not surface in English-language search?
4. Would you want the Argentina extension built as an optional module, or dropped entirely from the pipeline?
