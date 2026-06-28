# Watchlist Data Matrix v1 - Valuation QA

**Date:** 2026-06-28  
**Owner:** @ValuationReviewer  
**Reviewed file:** `reports/data-foundation/watchlist_data_matrix_v1_2026-06-28.md`  
**Task:** #investment-research task #10  

## Verdict

The matrix is fit for ResearchManager synthesis and screening as a source-first data foundation. It is not yet valuation-ready for L1 public-company mispricing conclusions because adjusted-close prices, share counts, market caps, enterprise values, and multiples are intentionally left blank.

The L1/L2 structure is mechanically consistent:
- L1 listed/public rows: 29
- L2 private/unlisted rows: 22

## What Passed

- Source-quality rules are clear: confirmed / reported / rumored / missing.
- L1 rows correctly avoid stale market prices and mark valuation metrics as missing pending adjusted-close refresh.
- L2 rows generally include valuation anchor, listing likelihood, private-company caveats, data gaps, and tracking metrics.
- Zhipu classification correction is carried forward: it should be treated as HK-listed China AI/model company, not pure private/unlisted.
- High-priority data gaps correctly identify the main blockers: adjusted-close price refresh, share count / EV refresh, AI revenue disclosure gaps, backlog/RPO conversion risk, private profitability/burn gaps, and China investability/policy risk.

## Required Before Any L1 Valuation Conclusion

For every L1 listed company, add a valuation refresh block with:

- adjusted close / 前复权 price
- price date and quote source
- share count source and date
- market cap
- cash, debt, minority interest/preferred where relevant
- enterprise value
- TTM revenue, EBITDA/operating income, net income, OCF, capex, FCF
- P/S, EV/Sales, P/E, EV/EBITDA, P/FCF, FCF yield
- if used, NTM/FY consensus multiples must be explicitly labeled as consensus-based
- FX basis for ADR/local listings such as TSM, Samsung, SK Hynix, Tencent, Alibaba, Zhipu/2513.HK

Until those fields are refreshed, use the matrix only for evidence screening and deep-dive prioritization, not for “cheap/expensive” conclusions.

## Required Before L2 Listing-Probability Conclusions

For every L2 private/unlisted company, add or standardize:

- valuation anchor date
- valuation source type: official funding / reported financing / secondary indication / prospectus / rumored
- security type and preferred terms, or explicit “unknown”
- latest disclosed or reported ARR/revenue date
- profitability/burn status: confirmed / reported / missing
- direct investability route: primary, secondary, public affiliate, future IPO only, not directly investable
- listing-likelihood rationale, not just high/medium/low
- listing blockers: governance, audit readiness, profitability, regulatory/geopolitical risk, capital intensity, customer concentration
- likely listing venue where relevant

## Structural Fixes Recommended

1. Add field-level source labels for mixed rows.
   Some public rows are partly confirmed and partly reported. AMZN and META are examples where transcript-specific or reported metrics should be field-level labeled rather than only row-level labeled.

2. Keep Zhipu in L1-E if 2513.HK status is valid.
   It should receive the same market-data refresh as public names: HKD adjusted close, share count, market cap, EV if possible, liquidity/free-float note, and Entity List / geopolitical caveat.

3. Keep Databricks as one L2 row with dual tags.
   The current dual role is appropriate: compute/cloud demand driver and IPO candidate. Avoid double-counting it in coverage totals.

4. Separate SpaceX from Starlink evidence where possible.
   Starlink prospectus/customer data and SpaceX private equity/secondary valuation are different evidence objects. Non-prospectus financial estimates should remain reported/secondary.

5. Add a listing-probability rubric.
   Proposed scale: High = prospectus/S-1/F-1 or active listing process; Medium-high = revenue scale + governance/investor base + credible IPO reporting; Medium = plausible but no formal process; Low = strategic tracking only.

6. Re-verify outlier private valuation anchors before using them in valuation work.
   Official financing announcements can be cited, but extreme headline valuations still require source/date/security-term checks before they drive listing-probability or mispricing analysis.

## Recommended Next Step

Proceed with ResearchManager screening using this matrix, but tag all L1 valuation conclusions as blocked until a dedicated market-data refresh is complete.

The next valuation task should be: “L1 adjusted-close / market cap / EV / multiples refresh for first deep-dive candidates.” Start with the recommended queue: NVIDIA, Microsoft, Alphabet, Amazon, Meta, Broadcom, TSMC, ASML.
