# Data Matrix Template & Merge Protocol v1

Date: 2026-06-28
Owner: @EvidenceAnalyst
Task: #investment-research task #8
Purpose: define the evidence/data matrix template, source-quality labels, and merge protocol for the L1/L2 AI-tech watchlist data foundation.

## Scope

Use the latest two-layer watchlist structure:
- L1: 29 listed targets.
- L2: 22 private/unlisted targets.

This task defines the data collection schema and merge rules only. It does not make investment conclusions.

Primary input already available:
- Evidence confirmation artifact: `reports/evidence/watchlist_evidence_confirmation_task9_2026-06-27.md`

## Core Matrix Schema

Use one row per company.

| Field | Required | Definition |
|---|---:|---|
| company | yes | Canonical company name. |
| layer_category | yes | L1-A to L1-E or L2-A to L2-D from the latest two-layer watchlist. |
| status | yes | listed / HK-listed / private / unlisted / expected IPO candidate / strategic tracking only. |
| investability | yes | direct common equity, ADR/H-share, ETF/supply-chain proxy, secondary/private access, listed affiliate, not directly investable. |
| AI_exposure | yes | Compute, cloud, model, app/software, data platform, robotics, defense, consumer distribution, semiconductor supply chain, energy/autonomy, etc. |
| source_links | yes | 3-5 core links, official first. |
| evidence_label | yes | confirmed / reported / rumored / missing, with mixed labels allowed by data item. |
| price_or_valuation_anchor | yes | Listed: adjusted close / 前复权 price, date, share count, market cap, EV. Private: latest round valuation / reported valuation / secondary indication / prospectus valuation. |
| latest_financials_or_ARR | yes | Listed: latest quarter and TTM financials. Private: ARR/revenue/funding/customer traction if available. |
| AI_option_evidence | yes | AI revenue, backlog/RPO, product ARR, model usage, GPU/ASIC/cloud capacity, enterprise traction, platform lock-in, distribution advantage. |
| valuation_metrics | yes for L1 | P/S, EV/Sales, P/E, EV/EBITDA, P/FCF or FCF yield. Use TTM unless explicitly tagged otherwise. |
| private_listing_likelihood | yes for L2 | high / medium / low / unclear, with reason. |
| private_discounts_caveats | yes for L2 | liquidity discount, transparency discount, preferred terms/liq pref unknown, secondary-market caveat. |
| market_implied_expectation | yes | What current price/valuation seems to imply: growth, margins, AI monetization, capex payback, IPO path, etc. |
| current_fundamentals_support | yes | What current verified fundamentals support, separated from option value. |
| data_gaps | yes | Missing or weak data needed before valuation or deep-dive conclusion. |
| tracking_metrics | yes | Metrics to refresh weekly/monthly/quarterly. |
| next_deep_dive_priority | yes | P0 / P1 / P2 or immediate / after data gap / strategic tracking. |
| next_update_trigger | yes | Earnings date, filing, funding, IPO filing, product launch, customer order, regulatory event, etc. |

## Source Quality Labels

### Confirmed
Use only for:
- SEC / exchange filings: 10-K, 10-Q, 20-F, F-1/S-1, HKEX filings, annual reports.
- Official company IR, earnings releases, investor presentations, transcripts hosted by company.
- Official company announcements, product docs, pricing pages, technical papers from the company.
- Government/regulator/contract award documents.

### Reported
Use for:
- Reuters, Bloomberg, WSJ, FT, The Information, CNBC, Nikkei, SCMP, credible industry publications.
- Credible third-party data providers or funding databases.
- Named investor/customer comments not in company filings.

### Rumored
Use for:
- Secondary-market indications without transaction documents.
- Anonymous-sourced valuation/revenue figures.
- Social media or unverified claims.

Rumored data must not drive the main valuation anchor. Put it in data gaps or appendix.

### Missing
Use when the variable is required for analysis but no reliable source is available.

## Listed Company Branch

Required fields for each L1 listed target:
- adjusted close / 前复权 price, price date, share count, market cap, EV.
- TTM revenue, gross margin, operating income/margin, net income, OCF, capex, FCF.
- cash, debt, buyback/dilution, R&D, capex/revenue.
- segment revenue where relevant.
- AI-specific proxy: data center revenue, AI semiconductor revenue, cloud AI growth, AI product ARR, RPO/backlog, AI capex, GPU/ASIC shipments, model/product usage.
- valuation metrics: P/S, EV/Sales, P/E, EV/EBITDA, P/FCF or FCF yield. Label TTM / NTM / FY consensus clearly.

Listed-company cautions:
- Backlog/RPO is not revenue.
- AI capex is not automatically AI revenue.
- Transcript-specific metrics need source tags if not in filings/IR tables.
- For China/HK names, explicitly tag listing venue, VIE/listing path if applicable, and policy/geopolitical risks.

## Private / Unlisted Branch

Required fields for each L2 target:
- latest funding round, amount, date, investors, valuation label.
- revenue / ARR / customer traction / usage, if available.
- model/product evidence, pricing/API docs, customer case studies, benchmarks.
- compute/capex indicators: GPU clusters, cloud commitments, data centers, training/inference cost clues.
- direct investability: private-only, secondary-market access, listed affiliate/proxy, IPO candidate, no direct path.
- listing likelihood: high / medium / low / unclear.

Listing-likelihood factors:
- audited or prospectus-ready financials.
- revenue/ARR scale and growth quality.
- governance/cap table maturity.
- major investor base and likely exit pressure.
- market window and comparable listings.
- regulatory/geopolitical constraints.
- profitability or credible path to profitability.
- customer concentration and legal/IP risk.

Private-company cautions:
- Funding valuation is a valuation anchor, not market price.
- Secondary valuation is not equivalent to public-market clearing price.
- Preferred-share terms, liquidation preferences, and structured rounds can distort headline valuation.
- Apply liquidity, transparency, and governance discounts explicitly.

## Merge Protocol

1. Start from task #9 evidence confirmation artifact.
2. Map every company to latest L1/L2 category from ResearchManager two-layer file.
3. Preserve existing source links and evidence labels from task #9.
4. Add missing financial/valuation fields:
   - L1: adjusted close, market cap, EV, TTM metrics, valuation multiples.
   - L2: listing likelihood, valuation anchor, investability path, discounts/caveats.
5. Do not overwrite labels upward. `reported` stays reported unless an official source is found.
6. For mixed rows, label at the data-item level inside the row, e.g. "confirmed for funding; reported for ARR; missing for profitability."
7. Add a data-gap summary by company.
8. Add a final cross-company gap list:
   - ready for immediate deep dive.
   - needs price/financial refresh.
   - needs private-company listing probability review.
   - strategic tracking only.

## Recommended v1 Delivery

File: `reports/watchlist_data_matrix_v1_2026-06-28.md`

Sections:
1. Scope and source rules.
2. L1 listed targets matrix.
3. L2 private/unlisted targets matrix.
4. Classification corrections.
5. High-priority data gaps.
6. Suggested next deep-dive queue.

## Known Classification Corrections

- Zhipu / Z.ai / Knowledge Atlas Technology should not remain in pure China private bucket if 2513.HK listing status is valid. Treat as HK-listed China AI/model company and keep liquidity, disclosure, Entity List, and geopolitical risk flags.
