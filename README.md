# Investment Research

AI/technology investment-research workspace focused on source-first data collection, watchlist construction, valuation QA, and mispricing deep dives.

## Current Status

As of 2026-06-28, the project has moved from target-list design into a usable v1 data foundation.

- Watchlist universe: 51 targets.
- L1 listed/public targets: 29.
- L2 private/unlisted targets: 22.
- Data matrix v1 is usable for screening and prioritization.
- L1 listed-company valuation conclusions still require a refreshed market-data pass for adjusted close, share count, market cap, EV, and valuation multiples.

## Key Files

### Watchlist

- `reports/watchlist/final_watchlist_two_layer_structure_2026-06-27.md` - latest two-layer L1/L2 watchlist structure.
- `reports/watchlist/final_canonical_watchlist_coverage_order_2026-06-27.md` - prior 51-target canonical coverage order.
- `reports/watchlist/ai_tech_target_watchlist_v1_canonical_2026-06-27.md` - canonical watchlist v1.
- `reports/watchlist/ai_tech_target_watchlist_v0_2026-06-27.md` - initial watchlist draft.

### Data Foundation

- `reports/data-foundation/watchlist_data_matrix_v1_2026-06-28.md` - current source-first data matrix.
- `reports/data-foundation/data_foundation_v1_manager_synthesis_2026-06-28.md` - manager synthesis and recommended next work.
- `reports/data-foundation/data_matrix_template_merge_protocol_v1_2026-06-28.md` - matrix schema, source labels, and merge rules.

### Evidence

- `reports/evidence/watchlist_evidence_confirmation_task9_2026-06-27.md` - merged evidence confirmation pass.
- `reports/evidence/private_app_robotics_defense_evidence_matrix_task13_2026-06-27.md` - private app, robotics, defense, and AI-product evidence lane.
- `reports/evidence/china_private_ai_evidence_matrix_task9_2026-06-27.md` - China private AI evidence lane and Zhipu classification correction.

### Valuation

- `reports/valuation/ai_tech_watchlist_valuation_framework_v1_2026-06-27.md` - valuation lenses and mispricing criteria.
- `reports/valuation/watchlist_data_matrix_v1_valuation_qa_2026-06-28.md` - QA of valuation fields and private-company caveats.

### MVP

- `reports/mvp/tsla_mvp_investment_report_2026-06-27.md` - TSLA MVP research-flow report.

## Recommended Next Work

Run two tracks in parallel:

1. L1 market-data refresh for `NVDA`, `MSFT`, `GOOGL`, `AMZN`, `META`, `AVGO`, `TSM`, `ASML`.
2. L2 listing-probability analysis for `Databricks`, `SpaceX/Starlink`, `ByteDance`, `OpenAI`, `Anthropic`, `Anysphere/Cursor`, `Anduril`, `Moonshot/Kimi`.

## Source-Quality Labels

- `confirmed`: company filing, company IR, company announcement, official docs, regulator source, or contract filing.
- `reported`: reputable media, credible data provider, or third-party estimate.
- `rumored`: unverified or secondary-market chatter.
- `missing`: required for analysis but not yet reliably sourced.
