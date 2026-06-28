# AI Investment Research Attack Directions Plan

Date: 2026-06-28
Owner: ResearchManager
Context: response to @huiru-gao direction list in #all:7a0b9d25.

## Executive View

We should start five parallel tracks:

1. CBRS / Cerebras deep review: newly public, high AI purity, low coverage, strong edge if disclosures are clean.
2. CRWV / CoreWeave deep review: backlog is the asset, but debt/capex/conversion risk decide whether it is real value or a story.
3. PLTR deep review: AIP is a high-disagreement software case; the key question is whether AI adoption is showing up in durable enterprise revenue.
4. Databricks listing tracker: not yet a direct listed trade, but an IPO/S-1 event can reprice SNOW, MSFT, AMZN, GOOGL and the data platform stack.
5. OpenAI IPO / valuation study: not directly investable yet, but it is the central private AI valuation anchor and demand source for MSFT, NVDA, ORCL, CRWV, CBRS and the broader AI capex chain.

Recommended attack order:

- Immediate listed deep dives: CBRS, CRWV, PLTR.
- Event tracking: Databricks S-1 readiness and OpenAI IPO/valuation.
- ResearchManager should own cross-company model architecture and final synthesis; EvidenceAnalyst should own source extraction; ValuationReviewer should own valuation / scenario model QA.

## Why These Can Produce PnL

The PnL source is not "AI is hot." The PnL source is expectation error:

- CBRS: the market may underwrite it as a niche AI chip IPO, while the real question is whether inference economics and OpenAI-related demand can scale into durable revenue.
- CRWV: the market may either over-trust headline backlog or over-penalize leverage. The trade depends on whether backlog converts into revenue and free cash flow fast enough to cover capex and interest.
- PLTR: the market debates whether AIP is real enterprise workflow adoption or hype. If AIP is embedded deeply enough, revenue duration and expansion may be under-modeled; if not, valuation can compress.
- Databricks: S-1 can reset public comps for SNOW and the cloud data/AI platform stack.
- OpenAI: its valuation affects private AI marks and public AI infrastructure names. The key is whether revenue growth, compute cost, gross margin and capital intensity can support the valuation.

## Data Collection And Cleaning Standard

Every company gets a facts table with these fields:

- company
- ticker / investability status
- metric
- period
- value
- unit
- GAAP / non-GAAP / company-defined
- source URL
- source tier
- extraction date
- as-of date
- confidence label: confirmed / company-reported / media-reported / estimated / rumored
- caveat
- related L1 / L2 mapping
- owner
- refresh cadence

Source tiering:

- Tier 1: SEC filings, prospectus, 10-Q/10-K, S-1, official investor relations releases, official annual reports.
- Tier 2: earnings call transcripts, official presentations, company blog posts with operating metrics.
- Tier 3: reputable financial media or analyst reports.
- Tier 4: secondary-market marketplaces, blogs, social media, anonymous reports. Use only as reported/rumored inputs, never as confirmed facts.

Cleaning rules:

- Separate GAAP, non-GAAP and company-defined metrics.
- Keep exact period labels: quarter, fiscal year, TTM, NTM, run-rate, ARR, backlog/RPO.
- Never mix ARR/run-rate with recognized revenue.
- Never mix revenue backlog, RPO and bookings without a bridge.
- For listed companies, use adjusted close / 前复权, diluted shares, market cap, EV and enterprise-value-based multiples.
- For private companies, use valuation anchors and liquidity/transparency discounts, not public equity multiples as if the shares were freely tradable.
- Preserve source caveats: customer concentration, related-party revenue, warrants/contra-revenue, pass-through revenue, preferred terms, lockups, IPO float and dilution.

## Models / Theory To Use

### Listed Company Base Model

- Expectations investing / reverse DCF: infer what growth, margin and FCF the market price already assumes.
- Scenario model: bear/base/bull with explicit probability weights.
- Growth-adjusted multiples: EV/Sales adjusted by revenue growth, gross margin, FCF margin and revenue durability.
- Unit economics: gross margin, capex intensity, FCF conversion, interest burden, customer concentration.
- Catalyst map: earnings, lockup, S-1 updates, customer contracts, capex announcements, regulatory events.

### CBRS / Cerebras

Key question: is CBRS a high-purity AI inference platform with durable economics, or a low-float IPO priced on excitement?

Data to collect:

- Revenue by hardware vs cloud/services.
- Gross margin by segment.
- OpenAI contract exposure, backlog and revenue conversion schedule.
- Customer concentration and receivables concentration.
- Warrant / contra-revenue treatment.
- Data center ownership, financing, leases and capex.
- Lockup schedule, float, insider selling, analyst coverage.

Model:

- Inference unit economics model: tokens/sec, cost per token, gross margin per workload, utilization.
- Customer concentration haircut.
- IPO dislocation / low-float volatility model.
- Reverse EV/Sales vs 2026-2028 revenue bridge.

Initial public facts to verify:

- Cerebras reported Q1 2026 GAAP revenue of $193.4M, up 94% year over year; GAAP gross margin 45%; GAAP net loss $14.0M; FY2026 core revenue outlook $855M-$865M.
- Source: https://investors.cerebras.ai/news-releases/news-release-details/cerebras-systems-announces-strong-first-quarter-2026-results

### CRWV / CoreWeave

Key question: is $99.4B backlog true contracted value, or mostly long-duration capital-intensive promise?

Data to collect:

- Backlog definition, RPO split, conversion timing.
- Recognized revenue, adjusted EBITDA, operating income and net loss.
- Capex plan, debt, interest expense, leases and liquidity.
- Customer concentration: Meta, Anthropic, Microsoft/OpenAI exposure if applicable, other AI labs.
- Power capacity: active power, contracted power, deployment timeline.
- GPU supplier dependency and NVIDIA relationship.

Model:

- Backlog-to-revenue waterfall.
- Backlog-to-EBITDA-to-FCF bridge.
- Debt service coverage and capex funding model.
- Customer concentration / termination risk haircut.
- Sensitivity to GPU price, utilization, power availability and refinancing cost.

Initial public facts to verify:

- CoreWeave reported Q1 2026 revenue of $2.078B, revenue backlog of $99.4B as of March 31, 2026, adjusted EBITDA of $1.157B, net loss of $740M, and interest expense net of $536M.
- Source: https://investors.coreweave.com/news/news-details/2026/CoreWeave-Reports-Strong-First-Quarter-2026-Results/

### PLTR / Palantir

Key question: is AIP becoming a durable enterprise operating layer, or is growth pulled forward by hype and government/large-contract concentration?

Data to collect:

- U.S. commercial revenue growth, customer count, TCV/RDV/RPO.
- Government revenue growth and contract duration.
- AIP bootcamp conversion and production deployment evidence.
- Net dollar retention / expansion metrics if disclosed.
- Gross margin, adjusted operating margin, FCF margin.
- Stock-based compensation and dilution.

Model:

- Land-and-expand cohort model.
- Government + commercial blended durability model.
- Rule-of-40 / FCF-adjusted software comp framework.
- Reverse DCF to determine what sustained growth and margin are priced in.

Initial public facts to verify:

- Palantir reported Q1 2026 U.S. revenue growth of 104% year over year and raised FY2026 revenue guidance; Q1 2026 U.S. commercial revenue was reported at $595M in the business update.
- Sources:
  - https://investors.palantir.com/news-details/2026/Palantir-Reports-Q1-2026-U-S--Revenue-Growth-of-104-YY-and-Revenue-Growth-of-85-YY-Raises-FY-2026-Revenue-Guidance-to-71-YY-Growth-and-U-S--Comm-Revenue-Guidance-to-120-YY-Crushing-Consensus-Expectations/
  - https://investors.palantir.com/files/Palantir%20-%20Q1%202026%20Business%20Update.pdf

### Databricks

Key question: if Databricks files or lists, does it reprice the cloud data platform market and create tradeable opportunities in SNOW/MSFT/AMZN/GOOGL?

Data to collect:

- S-1 status and filing changes.
- Revenue run-rate, ARR, growth, net retention, FCF.
- Data warehousing revenue, AI products revenue, Lakebase / Agent Bricks adoption.
- Customer count above $1M ARR.
- Competitive position versus Snowflake, Microsoft Fabric, Google BigQuery, Amazon Redshift, open source lakehouse.
- Valuation from latest primary or secondary round, with terms if available.

Model:

- IPO readiness scorecard.
- SaaS IPO comparable framework: EV/Sales vs growth, NRR, gross margin, FCF margin.
- Public comp spread vs SNOW / MDB / ESTC / cloud hyperscalers.
- Event path model: confidential S-1, public S-1, roadshow, pricing, first earnings after IPO.

Initial public facts to verify:

- Databricks announced >$4.8B revenue run-rate, >55% year-over-year growth, >$1B AI products revenue run-rate, >$1B Data Warehousing revenue run-rate, >140% net retention and a Series L valuing the company at $134B.
- Source: https://www.databricks.com/company/newsroom/press-releases/databricks-surpasses-4-8b-revenue-run-rate-growing-55-year-over-year

### OpenAI

Key question: can OpenAI's valuation be supported by revenue, margins and compute economics, or is it a capital-intensive growth story whose benefits accrue more reliably to suppliers?

Data to collect:

- ARR / revenue run-rate by year and latest quarter.
- User metrics: WAU, DAU, paid subscribers, enterprise customers, API usage.
- Revenue mix: ChatGPT consumer, Team/Enterprise, API, agents, ads/commerce.
- Compute capacity in GW, compute providers, committed spend, GPU mix.
- Gross margin and contribution margin by product if disclosed or inferable.
- R&D, inference cost, training cost, capex commitments, cash burn.
- Partner economics: Microsoft, Oracle, NVIDIA, CoreWeave, Cerebras, SoftBank.
- Governance, IPO path, S-1 status and legal structure.
- Valuation anchors: primary round, secondary trades, reported IPO target. Label every non-company number as reported/estimated.

Model:

- Compute-to-revenue flywheel: compute capacity -> model capability -> product usage -> revenue -> more compute.
- Unit economics per token / per user / per enterprise seat.
- Capital intensity model: revenue growth vs compute and R&D cash burn.
- Platform valuation framework: consumer + enterprise SaaS + API + ads/commerce optionality.
- Supplier pass-through map: how OpenAI growth translates into MSFT, ORCL, NVDA, CRWV, CBRS, AVGO, TSM.
- IPO valuation support test: required 2030 revenue, gross margin, FCF margin and terminal multiple needed to justify $500B / $850B / $1T scenarios.

Initial public facts to verify:

- OpenAI publicly stated revenue grew from $2B ARR in 2023 to $6B in 2024 and $20B+ in 2025, alongside compute capacity growth from 0.2 GW in 2023 to about 1.9 GW in 2025.
- Source: https://openai.com/index/a-business-that-scales-with-the-value-of-intelligence/

## Deliverables

Each subtask should produce:

1. Evidence table with source URLs and confidence labels.
2. Cleaned metric table in standardized units.
3. One-page thesis: bull / bear / key debate.
4. Model inputs and required valuation sensitivities.
5. Tradeability note: direct listed equity, supplier mapping, peer short/long, event-watch only.

ResearchManager final deliverable:

- Combined "first attack packet" ranking the five directions by edge, immediacy, data quality and tradeability.
