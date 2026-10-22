# PDFs needed

I cannot open any PDF from this container — WebFetch, curl and all direct HTTP are
blocked by the environment's network policy. Only a search tool works, and it returns
third-party summaries of abstracts. Every reference in the literature reviews is
therefore unverified at full-text level.

**Best fix: widen the network policy** (environment menu in the title bar → Edit →
Network access) to include `sciencedirect.com`, `ideas.repec.org`, `ssrn.com`,
`nber.org`, `imf.org`, `elibrary.imf.org`, `worldbank.org`, `onlinelibrary.wiley.com`,
`aeaweb.org`, `gov.br`, `anp.gov.br`, `comexstat.mdic.gov.br`, `cne.cl`,
`osinergmin.gob.pe`, `epe.gov.br`. Then I fetch these myself and verify the data
schemas too.

Drop PDFs in `01-brazil-supply-elasticity/literature/pdfs/` or
`02-stabilization-funds/literature/pdfs/` (both gitignored).

---

## Tier 0 — these four decide design questions, not just citations

1. **Vale, S.R. & Parente, V., "Time-Varying Elasticities in Brazil's Petroleum Trade:
   The Pre-Salt Paradox and Its Policy Implications"** (SSRN 6308961).
   *Why:* it claims capacity-constrained Brazilian production and a collapsed export
   price elasticity — both of Paper 1's proposed contributions. I need to know whether
   it identifies that or merely asserts it.
2. **"Rockets and feathers in the oil and gasoline markets: In-depth analysis of three
   asymmetries"** (ScienceDirect, 2026, S240585132600019X).
   *Why:* reportedly finds asymmetric thresholds and size-dependent nonlinear
   pass-through — Paper 2's Stage 2. Does it leave anything?
3. **Aastveit et al., "The price responsiveness of shale producers: Evidence from micro
   data," *Quantitative Economics* 2026** (doi 10.3982/QE2544). Open access.
   *Why:* I need the exact wording of its assumption that non-shale production does not
   respond to price. That sentence is Paper 1's opening.
4. **Kpodar & Abdallah, "Dynamic Fuel Price Pass-Through," IMF WP/16/254** or the 2017
   *Energy Economics* version.
   *Why:* is the 162-country Global Monthly Retail Fuel Price Database public, and does
   it cover the LatAm countries at usable frequency? If yes, Paper 2 should not rebuild
   prices at all.

**Plus: the special issue call itself.** I have never read it. Paste the scope text and
the operative deadline, or allow `sciencedirect.com`.

---

## Tier 1 — Paper 1 (Brazil offshore supply elasticity)

- Bjørnland, Nordvik & Rohrer, "Supply flexibility in the shale patch: Evidence from
  North Dakota," *Journal of Applied Econometrics* 2021 (doi 10.1002/jae.2808)
- Anderson, Kellogg & Salant, "Hotelling Under Pressure," *JPE* (~2018)
- Newell & Prest, "The Unconventional Oil Supply Boom," NBER WP 23973
- NBER WP 22532, "The Price-Responsiveness of Shale Gas"
- NBER WP 23423, "Lags, Costs, and Shocks: An Equilibrium Model of the Oil Industry"
- Kilian, "Facts and Fiction in Oil Market Modeling," *Energy Economics* 110 (2022) —
  or any working-paper version (CEPR DP14047 / Dallas Fed WP 1907 / CESifo WP 7902)
- Kilian & Murphy, *JAE* 2014; Baumeister & Hamilton, *AER* 2019
- Känzig, "The Macroeconomic Effects of Oil Supply News," *AER* 2021
- Caldara, Cavallo & Iacoviello, "Oil Price Elasticities and Oil Price Fluctuations," *JME*
- Dallas Fed WP 2609 (Apr 2026) and WP 2615 (Jun 2026) — free PDFs, I just cannot reach them
- Kellogg, "The Effect of Uncertainty on Investment," *AER* ~2014
- EPE, *Brazilian Oil & Gas Report*, 2021/22 through 2024/25 — free, English
- "The Brazilian 2010 oil regulatory framework and its crowding-out investment
  effects," *Energy Policy*
- The Hubbert curve-fitting paper on Brazilian post-salt production (S0920410517307209)

## Tier 1 — Paper 2 (stabilisation funds)

- Borenstein, Cameron & Gilbert, *QJE* 1997
- **"Retail Prices of Gasoline and Asymmetric Adjustment to Wholesale Prices in
  Colombia,"** *Journal of Economic Development* 2022
- **"Decomposition of Retail Gasoline Prices and the Sources of Market Power: Evidence
  for Colombia,"** Springer 2026 (doi 10.1007/s40812-026-00402-6) — paywalled
- IMF, "Automatic Fuel Pricing Mechanisms with Price Smoothing," TNM/12/03
- IMF WP/21/271, "The Distributional Implications of the Impact of Fuel Price Increases
  on Inflation"
- IMF WP/22/173, "Second-Round Effects of Oil Price Shocks"
- World Bank WPS 11153, "A Global Assessment of Domestic Petroleum Fuel Prices"
- World Bank WPS 6396, "Petroleum Product Pricing"
- World Bank, "Global Landscape of Fuel Subsidies and Price Controls," April 2025
- IMF chapter, "Domestic Petroleum Price Smoothing in Developing and Transition
  Countries" (the 45-country survey, incl. the Chile FEPP 2003 failure)
- Pham, "Can the Oil Price Stabilisation Fund Reduce the Volatility of Domestic
  Prices?", *Asia & the Pacific Policy Studies* 2025
- IMF Chile technical assistance report, 2023 (MEPCO)
- Kilian & Zhou on gasoline prices, oil prices and inflation expectations, *JAE* ~2022
- Cebotari, "Contingent Liabilities: Issues and Practice," IMF WP/08/245
- Polackova, World Bank Policy Research WP 1989
- Hansen, threshold regression (*Econometrica* ~1996, ~2000)
- MacKinnon & Webb, wild cluster bootstrap with few clusters

## Tier 2 — useful, not blocking

- ANP data dictionaries for the well-level production datasets
- Petrobras *Plano Estratégico* documents, 2010–2026
- WTO presentation, "Chile's Policy Response to the 2026 International Fuel Price Shock"
- SEI, "A Strategic Phase-out of Colombia's Diesel Subsidy" (2024)
- 9ELAEE paper on FEPC institutional design
- Fedesarrollo, *Tendencia Económica* no. 226
- Oxford Energy Forum issue 149 (May 2026)
- World Bank *Commodity Markets Outlook* 2026
