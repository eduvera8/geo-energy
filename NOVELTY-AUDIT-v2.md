# Novelty audit v2 — supersedes the verdicts in `EXTENDED-ABSTRACTS.md` §I.3

**Date:** 22 October 2026
**Why this exists:** the v1 novelty check was a general-web scan, not a literature search. Redone with domain-restricted queries against RePEc, NBER, SSRN, ScienceDirect, Wiley, IMF eLibrary and World Bank. **Two of my earlier conclusions were wrong.** This file records what changed and what the standard of evidence actually is.

---

## 1. What this audit can and cannot establish

**Method used:** the search tool with `allowed_domains` restricted to scholarly hosts, returning titles, URLs and a third-party summary of each result. Twelve queries across the two papers.

**What I still cannot do, and therefore cannot claim:**

| Limitation | Consequence |
|---|---|
| No full-text access to any paper | Cannot confirm what a paper actually estimates, on what sample, with what result. All claims below are abstract-level at best, and several are a summarizer's paraphrase of an abstract. |
| No EconLit, Google Scholar, Web of Science, Scopus | No systematic coverage. A general index plus domain restriction is a screen, not a search. |
| No citation chaining | Cannot trace forward or backward from a key paper, which is how pre-emption is normally found. |
| No reliable coverage of working papers under review | A paper on the 2026 shock could be in the pipeline at any of five journals and be invisible to me. |
| Summarizer can misattribute | Authors, years and numbers below may be wrong even when the paper exists. |

**The correct standard for everything below is "no evidence found in accessible indexes."** It is not "novel." Closing that gap requires one of: widening this environment's network policy, you running Scholar/EconLit yourself, or you sending PDFs.

---

## 2. Paper 1 (Brazil offshore supply elasticity) — gap holds, one competitor appears

### 2.1 The core gap survived a proper screen

Domain-restricted search for offshore or deepwater supply elasticity returned **no estimate for offshore production anywhere**. The confirmed landscape:

| Reference | Status | Finding |
|---|---|---|
| Bjørnland, Nordvik & Rohrer, *JAE* 2021, "Supply flexibility in the shale patch: Evidence from North Dakota" (doi 10.1002/jae.2808) | **Confirmed, incl. journal and year** | Shale well elasticity 0.3–0.9; no conventional response |
| Aastveit et al., *Quantitative Economics* 2026, "The price responsiveness of shale producers" (doi 10.3982/QE2544) | **Confirmed** | Shale short-run elasticity **up to 0.62**; global short-run elasticity **~0.06–0.07** derived by assuming shale is ~10% of output and **"the rest of oil production is conventional and does not promptly respond to oil price changes"** |
| Newell & Prest, NBER WP **23973**, "The Unconventional Oil Supply Boom" | **Confirmed** | Drilling response ~1.6%/1% price for tight oil, ~1.2% for conventional |
| Anderson, Kellogg & Salant (Texas well-level) | Confirmed in substance | The margin that matters is **drilling investment**; production from existing wells barely reacts |
| NBER WP **22532**, "The Price-Responsiveness of Shale Gas" | Newly found | Not previously on my list |
| NBER WP **23423**, "Lags, Costs, and Shocks: An Equilibrium Model of the Oil Industry" | Newly found | Structural treatment of investment lags — a theory-side competitor. Authors unverified (I believe Bornstein, Krusell & Rebelo) |
| Survey evidence | Confirmed in substance | Short-run supply elasticities span **0–0.27**; "supply elasticity studies are rare compared with demand studies" |

**This is the strongest possible version of the gap.** The frontier paper (Aastveit et al. 2026) *states as an explicit assumption* the thing my paper would test: that non-shale production does not promptly respond to price. Quote that assumption in the introduction and the contribution writes itself.

### 2.2 The competitor I missed in v1

**Vale, S.R. & Parente, V., "Time-Varying Elasticities in Brazil's Petroleum Trade: The Pre-Salt Paradox and Its Policy Implications," SSRN.** TV-VAR on monthly data 2003–2025. Reported finding: **export price elasticity collapsed by 71.5%, "reflecting capacity-constrained production operating regardless of price fluctuations."**

That claims both of the things I proposed as Paper 1's contributions — the capacity constraint and the export/allocation margin — for Brazil.

**Assessment: a positioning problem, not a kill.**
- It is SSRN; peer-review status unknown. Possibly unpublished or under review.
- It uses TV-VAR on aggregate trade flows. That is the method family this issue's editors disfavour, and it cannot identify a capacity constraint — it can only observe that an elasticity fell, then assert capacity as the interpretation.
- It has no well-level data, no production-unit nameplate capacity, no separation of extensive from intensive margins, and no identified shock.
- So the claim is **asserted** where my design would **identify** it. That is a strong position to be in: a referee who knows this paper will want exactly the properly identified version.

**Required action: I need this PDF.** If it already identifies the capacity constraint credibly, Paper 1 needs reframing. I cannot tell from a search snippet.

### 2.3 Other Brazil-specific work found

- A curve-fitting study of Brazilian offshore post-salt output: deviations from a Hubbert curve track oil price changes with a **four-to-five year lag**. Supports the near-zero short-run response prior, and means someone has looked at Brazilian supply response, if crudely.
- *Energy Policy*: "The Brazilian 2010 oil regulatory framework and its crowding-out investment effects."
- Documented claim that the **2011–2014 domestic fuel price controls damaged Petrobras's financial position and hampered pre-salt investment**. This confirms the NOC confound is real and documented — and points to a sharper design: identify the investment response through **cash flow and leverage**, not price alone.

### 2.4 Revised verdict, Paper 1

| Dimension | v1 | v2 | Why |
|---|---|---|---|
| Novelty | 5 | **4.5** | Core gap confirmed and sharpened; one SSRN competitor on the framing |
| Data | 5 | **4** | FPSO crosswalk and futures-curve instrument are unresolved risks (see `01-brazil-supply-elasticity/DATA-PLAN.md` §3–4) |
| Fit | 5 | **5** | Supplies the parameter the editors' own scenario models assume |

**Still the clear first choice.**

---

## 3. Paper 2 (stabilisation funds) — substantially pre-empted

This is where I was wrong, and the damage is significant.

### 3.1 Cross-country pass-through: already done, with a better database than I proposed building

| Reference | Finding |
|---|---|
| **Kpodar & Abdallah, IMF WP/16/254 (2016)**, published in *Energy Economics* 2017: "Dynamic fuel price pass-through: Evidence from a new global retail fuel price database" | **162 countries, monthly, local projections.** Hump-shaped pass-through peaking within 3–6 months. **Positive oil shocks pass through faster and more strongly than negative ones** — the asymmetry already established. (WP and journal versions report different headline numbers: 1.2 cents at six months vs 0.7 cents at three. Cite carefully.) |
| **IMF WP/21/271 (2021)** | Updated Global Monthly Retail Fuel Price Database. Peak pass-through in advanced economies **double** that in developing economies; transmission more protracted in the latter. |
| **World Bank WPS 11153**, "A Global Assessment of Domestic Petroleum Fuel Prices" | Eight fuels, 2017–2023. Net exporters have the lowest pass-through; advanced countries the highest. |

My proposed Stage 1 — cross-country asymmetric pass-through on a common benchmark — is **done, at global scale, by the IMF, twice, with a purpose-built 162-country database.** Rebuilding a six-country weekly panel to re-estimate it is not a contribution.

### 3.2 Tail-state rule breakdown: pre-empted by a 2026 paper

**"Rockets and feathers in the oil and gasoline markets: In-depth analysis of three asymmetries,"** ScienceDirect, 2026. Reported findings: a clear **inaction band with asymmetric thresholds**; prices adjust quickly to small increases but require much larger decreases before cuts; and **asymmetry arises primarily through nonlinear impulse responses, with large positive shocks passed through more rapidly and completely than negative shocks.**

That is my Stage 2 — size-dependent, threshold, nonlinear pass-through with large shocks — published this year. Authors and data source unconfirmed from the snippet. **I need this paper.**

Related: **IMF WP/22/173** finds shocks during large oil price booms have *weaker* pass-through to wages, attributed to retail energy market structure dampening large swings — which cuts against my predicted direction and must be addressed.

### 3.3 Fund failure under high prices: documented precedent

- An IMF chapter surveying **45 developing countries** finds roughly a quarter of price-regulating countries operate stabilisation funds, and that **some were later abolished over their fiscal costs**.
- **Chile's FEPP went bust in 2003** after the late-1990s oil price increase nearly depleted it. So "the rule breaks in the tail" has a documented historical instance in one of my own sample countries.
- **IMF TNM/12/03, "Automatic Fuel Pricing Mechanisms with Price Smoothing"** (2012) — the design manual for exactly these rules, which I had entirely missed.
- **World Bank WPS 6396, "Petroleum Product Pricing"** — identifies the countries operating such funds (Colombia, Malawi, Morocco, Nigeria, Peru, Thailand, Vietnam) and flags Nigeria's as requiring the largest budget transfers.
- **Pham (2025), *Asia & the Pacific Policy Studies*, "Can the Oil Price Stabilisation Fund Reduce the Volatility of Domestic Prices?"** — finds fund effectiveness at price stabilisation **limited**, with more pronounced distributional effects.
- **IMF blog, 18 June 2026, "The Energy Shock Is Testing Government Budgets"** — warns that price caps by oil-importing countries **risk becoming impossible to finance** if prices escalate further. **The IMF is already publishing on Paper 2's exact policy question, in 2026.**

### 3.4 What survives: the option valuation, and only that

A targeted search for option-pricing or contingent-claims valuation of consumer fuel price caps **again returned nothing**. The adjacent real-options literature values *subsidies that induce investment* (binomial valuation of Chinese renewable subsidies, *Energy Economics* 2020; carbon price floors valued by Least Squares Monte Carlo) and the generic put-option framing appears in valuation references. **Nobody appears to value a consumer fuel price cap as an uncovered short option written by the sovereign.** That part held up across two independent queries.

### 3.5 Revised verdict, Paper 2

| Dimension | v1 | v2 | Why |
|---|---|---|---|
| Novelty | 4 | **2.5** | Stage 1 done by IMF ×2 and World Bank; Stage 2 done by a 2026 paper; fund failure documented; IMF already on the 2026 question. Only the valuation survives. |
| Data | 5 | **5** | Unchanged, and now partly unnecessary |
| Fit | 5 | **4.5** | Still the editors' topic area, but a crowded corner of it |

**Paper 2 as specified is no longer worth writing.** Three options:

**(a) Narrow it to the valuation — my recommendation if you keep it.** Drop the pass-through re-estimation entirely. Use the IMF's existing retail price database (check whether it is public) plus hand-coded rule parameters, and contribute *only* the derivative framing: what option each rule represents, what 2026 cost each sovereign, what the fair ex-ante premium was, and what hedging it would have cost against Mexico's sovereign hedge as the benchmark. Shorter paper, far cheaper to execute, one clean contribution. **Tension you should weigh: this makes it a finance and fiscal-accounting paper, not an econometrics paper — which cuts against your stated requirement.**

**(b) Swap it.** The Venezuela/two-shocks paper (`EXTENDED-ABSTRACTS.md` Part IV) had no pre-emption at all in either audit round and remains structurally econometric. Its weakness is the Venezuelan barrel count, which I proposed handling with bounds rather than assumptions.

**(c) Keep both as written** — against my advice, now that Stages 1 and 2 are taken.

---

## 4. Consolidated ranking, v2

| Rank | Paper | Data | Fit | Nov | Weighted (0.40/0.35/0.25) |
|---|---|---|---|---|---|
| **1** | Brazil offshore supply elasticity | 4 | 5 | 4.5 | **4.48** |
| 2 | Venezuela + war, state dependence | 3.5 | 5 | 5 | **4.40** |
| 3 | Gas shock × hydrology → power | 4.5 | 4 | 4.5 | 4.33 |
| 4 | Stabilisation funds, **narrowed to valuation** | 5 | 4.5 | 3.5 | 4.45 |
| 5 | Stabilisation funds **as originally specified** | 5 | 4.5 | 2.5 | 4.20 |

Rows 1, 2 and 4 are within 0.08 of each other, which is noise given that every input is a judgement call. The defensible statement is: **Paper 1 is the clear first pick; the second slot is a genuine three-way choice**, and the deciding factor should be which data risk you would rather carry — the FPSO crosswalk (Paper 1 companion), the Venezuelan barrel count, or paywalled JKM.

---

## 5. What I need from you to close this properly

**Highest value: widen the network policy.** With `sciencedirect.com`, `ideas.repec.org`, `ssrn.com`, `nber.org`, `imf.org`, `worldbank.org`, `gov.br`, `anp.gov.br` and `comexstat.mdic.gov.br` allowed, I could read these papers instead of guessing at them, and verify the data schemas myself. That single change removes most of the uncertainty in this file.

**Failing that, four PDFs decide real questions** (full list in `PDF-REQUESTS.md`):

1. **Vale & Parente, SSRN, "Time-Varying Elasticities in Brazil's Petroleum Trade: The Pre-Salt Paradox"** — does it already own Paper 1's capacity and export-margin claims?
2. **"Rockets and feathers in the oil and gasoline markets: In-depth analysis of three asymmetries," 2026** — does it already own Paper 2's Stage 2?
3. **Aastveit et al., *QE* 2026** — open access; I need the exact statement of the non-shale assumption to quote.
4. **Kpodar & Abdallah, IMF WP/16/254 or the 2017 *Energy Economics* version** — is their database public, and does it include the LatAm countries at the frequency Paper 2 would need?

**And the special issue call itself.** I have still never read it. Paste the scope text and the deadline, or allow `sciencedirect.com`.
