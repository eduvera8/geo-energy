# Fresh-start prompt

Copy everything below the line into a new Claude Code session, run from a **clean
directory** (or delete this repo's existing analysis files first — they came from a
session with no internet access and their conclusions are unreliable).

---

I'm an economist. I want to write one high-quality paper for the *Energy Economics*
special issue "The Role of Geopolitics in Energy Markets" (ScienceDirect special issue
334954; guest editors Lutz Kilian, Michael D. Plante, Siquan Wang). I have a strong
preference for a Latin America angle but will drop it if a better idea exists. The paper
must have serious econometrics — credible identification, not index-on-returns
regressions.

You have web access. Use it. Read primary sources rather than summaries of them.

## Non-negotiable standards

1. **Never state that something is novel, or that a gap exists, on the basis of search
   snippets.** Distinguish three evidence levels explicitly every time you make a
   novelty claim: (a) I read the full text; (b) I read the abstract; (c) a search result
   mentioned it. Search Google Scholar, RePEc/IDEAS, SSRN, NBER, journal sites and
   EconLit if you can reach it, and do forward/backward citation chaining on the two or
   three closest papers. If you cannot verify, say "no evidence found in the indexes I
   could reach" and name which ones.
2. **Verify data before designing around it.** Do not propose a design that depends on a
   dataset until you have confirmed it exists, is downloadable, covers the needed period
   and frequency, and has the variables you need. Open the portal, download a sample,
   print the schema. A design built on an assumed dataset is worthless.
3. **Feasibility means statistical power, not researcher time.** Specifically: the 2026
   shock began in late February 2026, so an aggregate monthly outcome gives roughly
   eight post-shock observations. When a shock is common to all units, cross-sectional
   size does not substitute for time-series length — N buys precision on a time effect,
   not identification. So any viable design must get identification from one of:
   differential pre-determined exposure across units; a long estimation sample with 2026
   used only out of sample; or high-frequency data with many separately dated shocks.
   State which one applies for every candidate idea.
4. **Tell me when you can't do something.** If a site is blocked, a paper is paywalled,
   or a dataset isn't public, say so immediately and tell me what you need from me.
   Don't work around it silently and don't substitute a guess.
5. Flag uncertainty in proportion to the evidence. I would rather hear "I'm not sure,
   here's what would settle it" than a confident wrong answer.

## Work in this order

**Phase 0 — read the call.** Fetch the special issue page and the journal's call for
papers. Get the actual scope text, the submission window (Elsevier pages have carried
conflicting deadlines, so resolve it), and any special instructions. Quote the scope
verbatim in your notes. If the page is inaccessible, tell me and I'll paste it.

**Phase 1 — the editorial filter.** Work out what this specific editorial team rewards
and rejects, from their own published work, not from generic advice about publishing.
Read Kilian's *Facts and Fiction in Oil Market Modeling* (*Energy Economics* 110, 2022)
and at least two recent Plante papers. Check what the Dallas Fed has already published
on the 2026 disruption — if the editors' own institution has covered a question, a paper
competing with it will lose, and the complementary move is to supply a parameter their
models have to assume. Write this up as an explicit do/don't list before generating
ideas.

**Phase 2 — the 2026 factual record.** Build a primary-sourced chronology of the shock:
the Iran war's onset, the Strait of Hormuz closure and its status, price path, OPEC and
Gulf producer responses, IEA stock release, and the Venezuela sanctions/regime sequence
of Dec 2025 – Feb 2026. Use OFAC notices, IEA and OPEC publications, EIA data and
central bank sources. Secondary reporting conflicts on several of these, including the
Venezuelan timeline — note conflicts rather than picking one silently. Also date the
individual news events of the episode: the war generated many separately datable shocks
between February and October 2026, which matters for high-frequency identification.

**Phase 3 — data inventory.** Before generating ideas, inventory what energy data is
actually available at better than annual frequency for the regions in scope, and
*verify* each entry by opening it. Cover at minimum: upstream production microdata
(well/field level) from national regulators; retail fuel price surveys; power system
spot prices and dispatch; customs microdata; refinery throughput; futures and options
settlements; freight (note which of Baltic/Clarksons/Kpler are licensed rather than
free). Report coverage, frequency, unit of observation, variables and how to download
each. This inventory determines which ideas are real.

**Phase 4 — generate and screen.** Produce 15–20 candidate papers. Score each on data
adequacy, fit with the editorial filter, and novelty, with explicit weights, and state
which identification route (per standard 3) each uses. Then run a real literature search
on the top five before narrowing further — do not narrow on the basis of my priors or
yours. Expect to kill ideas at this stage; tell me which and why.

**Phase 5 — design.** For the best two or three, write extended abstracts that make
crystal clear: the single main point in one paragraph; exactly what data, with
verification status; the estimating equations; the identification argument and its
threats; the inference strategy; what result would falsify the thesis; and what could
kill the project. Recommend one, with reasoning, and name the deciding factor.

**Phase 6 — execute** the one I pick: acquire and clean the data, build the panel, run
the estimation, and write the paper. Keep raw data out of version control and make every
step reproducible from a manifest of sources.

## Unverified leads from an earlier session — verify or discard, do not trust

These came from a session with **no internet access**, working only from a search tool
that returned third-party summaries. Several claims made there turned out to be wrong.
Treat every item below as a hypothesis to check, not as an input. **If verifying one is
expensive, discard it and work from your own search instead.**

- The frontier micro-estimates of short-run oil supply elasticity may all be US-based
  (North Dakota, Texas: Bjørnland–Nordvik–Rohrer *JAE* 2021; Aastveit et al. *QE* 2026;
  Newell–Prest NBER 23973; Anderson–Kellogg–Salant). The global short-run elasticity in
  common use (~0.06–0.07) may rest on an explicit assumption that non-shale production
  does not respond to price. If that is right, estimating it for a non-US, non-shale
  producer is a parameter contribution. Check whether any offshore estimate exists.
- Possible competitor on that: Vale & Parente, "Time-Varying Elasticities in Brazil's
  Petroleum Trade: The Pre-Salt Paradox," SSRN. Read it and judge whether it forecloses
  the question.
- Cross-country fuel price pass-through appears well covered (Kpodar & Abdallah, IMF
  WP/16/254 and *Energy Economics* 2017, with a 162-country monthly database; IMF
  WP/21/271; World Bank WPS 11153), and a 2026 paper may already cover size-dependent
  threshold pass-through. Valuing a consumer fuel price cap as an uncovered short option
  written by the sovereign appeared *not* to be covered — verify before building on it.
- Dallas Fed WP 2609 (Apr 2026) and WP 2615 (Jun 2026) appear to model the Hormuz
  closure. Read them first; they define what not to duplicate.
- Latin America plausibly contains both sides of this shock: Brazil, Guyana, Argentina
  and Colombia as beneficiaries; Chile, Peru, Central America and the Caribbean as
  exposed importers; Mexico's product import bill reportedly exceeding crude export
  earnings for the first time in decades; Brazil reportedly sourcing a large share of
  fertiliser through Hormuz. All of these need checking against primary data.
- Plausibly useful data, all unverified: ANP (Brazil) well- and field-level monthly
  production and its weekly retail fuel price survey; Argentina's Secretaría de Energía
  well-level production and fracture registry; Comex Stat monthly customs microdata;
  hourly power market data from CCEE/ONS, CAMMESA, Coordinador Eléctrico and XM; EIA
  weekly imports by origin and PADD refinery data; CME settlements. Also unverified:
  whether ANP's well-level file identifies the production unit each well flows to, and
  whether any free source provides daily futures *curve* data.

## How I want you to work

- Ask me when a choice is genuinely mine; otherwise decide and tell me what you decided.
- Push back if I'm wrong, including about my own field or my country preferences. If I
  overrule you, do it my way and note the cost once.
- Correct your own errors plainly and move on. Don't pad.
- Keep deliverables as files in the repo: a notes file per phase, a source manifest, and
  code that reruns end to end.
- Tell me early and specifically what you need from me: PDFs behind paywalls, documents
  in Spanish or Portuguese that need a human, institutional data subscriptions, or
  judgement calls on scope.

Start with Phase 0 and report back before moving on.
