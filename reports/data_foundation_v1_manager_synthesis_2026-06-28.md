# Data Foundation v1 - Manager Synthesis

Date: 2026-06-28
Owner: @ResearchManager

Inputs:
- Two-layer watchlist: `reports/final_watchlist_two_layer_structure_2026-06-27.md`
- Data matrix v1: `/Users/sjin/.slock/agents/6dbffcc0-c910-4ee6-97ea-736e4a918272/reports/watchlist_data_matrix_v1_2026-06-28.md`
- Valuation QA: `/Users/sjin/.slock/agents/9fe4b418-f779-408f-b283-2db54e8d8735/reports/watchlist_data_matrix_v1_valuation_qa_2026-06-28.md`

## Status

The project has moved from watchlist design into a usable source-first data foundation.

What is complete:
- L1/L2 watchlist taxonomy is fixed.
- Evidence matrix template and merge protocol are complete.
- Data matrix v1 is complete for all 51 targets.
- Valuation QA confirms the matrix is fit for screening and synthesis.
- L1/L2 row counts are mechanically consistent: L1 = 29, L2 = 22.
- Zhipu classification correction is carried forward: HK-listed China AI/model company, 2513.HK / Knowledge Atlas Technology.

What is not complete:
- L1 public-company valuation conclusions are not yet ready.
- Adjusted close, share count, market cap, EV, and valuation multiples still need a refreshed market-data pass.
- Some L2 private-company valuation anchors still require source/date/security-term verification.

## What We Can Do Now

The current matrix is ready for:
- Screening the research universe.
- Selecting the first deep-dive candidates.
- Identifying key evidence gaps and tracking metrics.
- Designing valuation-refresh tasks.
- Starting L2 private AI listing-probability work.

The current matrix is not ready for:
- Calling L1 public names cheap or expensive.
- Producing final valuation ranges.
- Comparing private valuation marks directly against public market caps.

## Immediate Workstreams

### Workstream A: L1 Market-Data Refresh

Purpose: make public-company rows valuation-ready.

Start with the first eight L1 names:
1. NVIDIA
2. Microsoft
3. Alphabet
4. Amazon
5. Meta
6. Broadcom
7. TSMC
8. ASML

Required fields:
- adjusted close / 前复权 price
- price date and source
- share count and source date
- market cap
- cash and debt
- enterprise value
- TTM revenue
- EBITDA or operating income
- net income
- OCF, capex, FCF
- P/S, EV/Sales, P/E, EV/EBITDA, P/FCF, FCF yield
- FX basis for ADR/local listings

Output:
- `l1_market_data_refresh_batch1_YYYY-MM-DD.md`

### Workstream B: L2 Listing Probability Analysis

Purpose: determine which private/unlisted names can become investable events or affect L1 valuation assumptions.

Start with:
1. Databricks
2. SpaceX / Starlink
3. ByteDance
4. OpenAI
5. Anthropic
6. Anysphere / Cursor
7. Anduril
8. Moonshot AI / Kimi

Required fields:
- current status
- latest valuation anchor and source label
- latest revenue/ARR evidence and source label
- direct investability route
- likely listing path
- likely listing venue
- listing probability
- expected horizon
- main listing blockers
- main public proxy / affected L1 names
- what would change the probability

Output:
- `l2_listing_probability_batch1_YYYY-MM-DD.md`

### Workstream C: Deep-Dive Queue Selection

Purpose: choose the first 3-5 names for full research reports.

Recommended default queue:
1. NVIDIA
2. Microsoft
3. Alphabet
4. Databricks
5. OpenAI

Rationale:
- NVIDIA, Microsoft, Alphabet are the largest direct public mispricing debates.
- Databricks is both a private IPO candidate and a pressure point for Snowflake/cloud platform assumptions.
- OpenAI is the most important private AI valuation mark and directly affects Microsoft, cloud AI capex, and AI infrastructure demand.

## Recommended Next Decision

Ask @huiru-gao / @shendan-jin to choose one of these:

1. **Public-first:** run L1 market-data refresh for the first eight public names, then start NVIDIA deep dive.
2. **Private-first:** run L2 listing probability analysis for the first eight private names.
3. **Parallel:** run public market-data refresh and private listing-probability analysis at the same time.

Manager recommendation: choose **Parallel** if agent capacity is available. It gives the fastest path to both tradable public opportunities and private-event intelligence.

## PnL Logic

The likely PnL does not come from having a list. It comes from catching expectation gaps:

- Public companies where AI evidence is stronger than market-implied assumptions.
- Public companies where market is overpaying for distant option value not yet supported by data.
- Private companies whose funding, IPO, product traction, or customer signals change how public comps should trade.
- Supply-chain names where demand durability, backlog conversion, or capex timing is misunderstood.

The data foundation is the filter that turns the broad AI narrative into comparable, evidence-backed mispricing candidates.
