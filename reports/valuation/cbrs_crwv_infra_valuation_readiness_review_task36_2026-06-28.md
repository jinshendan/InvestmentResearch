# CBRS / CRWV Infrastructure Valuation Readiness Review

**Date:** 2026-06-28  
**Owner:** @ValuationReviewer  
**Task:** #36 review of tasks #31/#32 valuation gates  
**Reviewed artifacts:**  
- `reports/deep-dive/cbrs_cerebras_deep_review_v1_2026-06-28.md`  
- `reports/deep-dive/cbrs_cap_table_contract_bridge_task31_2026-06-28.md`  
- `reports/deep-dive/crwv_coreweave_deep_review_v1_2026-06-28.md`  
- `reports/deep-dive/crwv_rpo_fcf_bridge_task32_2026-06-28.md`

## Verdict

The task #31 and task #32 follow-up work is the right next layer, and both artifacts are usable for manager synthesis. They correctly prevent the two biggest valuation errors:

1. **CBRS:** capitalizing the >$20B OpenAI contract or $25.0B RPO before solving dilution, warrant amortization, tranche-level revenue, data-center obligations, and tradable float.
2. **CRWV:** treating $99.4B revenue backlog / $98.8B RPO as equity value before deducting capex, depreciation, debt, interest, and execution risk.

My valuation view: neither CBRS nor CRWV is trade-memo ready from headline revenue/backlog alone. CRWV is closer to a modelable public valuation because the RPO timing buckets, debt principal, interest expense, PP&E purchases, and EBITDA bridge are already explicit. CBRS may have a larger information-edge setup, but the fully diluted cap table and contract economics are not solved enough for per-share valuation.

## CBRS Readiness Review

CBRS should be framed as a scarce public AI-inference infrastructure option, not a simple revenue multiple trade.

| Gate | Current evidence | Review |
|---|---|---|
| Revenue base | Q1 GAAP revenue $193.4M; FY26 core revenue guide $855M-$865M. | Use FY26 guide as the first anchor. Do not annualize one quarter as the main case. |
| OpenAI contract | 750MW committed capacity over 2026-2028; option for another 1.25GW by 2030; company says value is >$20B. | Confirmed and important, but not yet revenue, cash flow, or equity value. |
| RPO | $25.0B remaining performance obligations. | Central to bull case, but must be split into OpenAI vs non-OpenAI, timing, margin, and cancellation/acceptance risk. |
| OpenAI recognized revenue | $16.9M Q1 revenue net of $0.8M warrant amortization. | This is the cleanest proof that headline contract value is far ahead of current recognized revenue. |
| Customer concentration | Two 10%+ revenue customers were 63% and 11% of Q1 revenue; three customers were 86% of AR. | Requires a concentration discount until non-OpenAI/G42/AWS revenue scales. |
| Dilution | OpenAI warrant up to 33.445M Class N shares; G42 warrant exercised in Q2; SBC/options/RSUs and post-IPO share count unresolved. | This blocks per-share valuation. Fully diluted market cap must include customer warrants. |
| Capital obligations | Q1 non-commenced lease commitments about $2.3B plus Q2 additional commitments about $1.6B. | Contract conversion depends on capacity buildout and lease/capex funding, not just demand. |
| Liquidity/tradeability | IPO closed May 2026; lock-up, float, ADV, options liquidity, and borrow availability remain data gaps. | This blocks position sizing and short/hedge analysis. |

### CBRS Valuation Position

The correct interim conclusion is **high-potential edge, not valuation-ready**.

The market can reasonably assign option value to a newly public AI-inference asset tied to OpenAI, but the valuation cannot rely on `headline contract / current revenue` or `RPO / guide` alone. The next model must be a contracted-revenue-to-gross-profit-to-fully-diluted-per-share bridge:

| Model step | Required input |
|---|---|
| OpenAI revenue schedule | Tranche-level capacity acceptance, annual minimums, timing, cancellation/delay clauses. |
| Revenue quality | OpenAI/G42/AWS vs other customers; committed vs option vs expected renewal. |
| Gross profit | Hardware vs cloud/services mix, data-center/power costs, customer-level margin. |
| Operating loss path | FY26 core operating margin guide negative 28%-32% and opex scale. |
| Dilution | Post-IPO basic shares, OpenAI/G42/customer warrants, RSUs/options/SBC, any partner equity. |
| Enterprise value | Fully diluted market cap plus debt/debt-like leases less pro forma cash. |
| Tradeability | Float, lock-up expiry, ADV, options open interest, borrow cost. |

### CBRS Mispricing Thesis

Bull case:
- The market underprices a scarce public inference-infrastructure company with direct OpenAI demand exposure.
- OpenAI capacity tranches convert on schedule and visible revenue ramps in 2H26/2027.
- Warrant dilution and amortization are manageable relative to realized gross profit.
- Non-OpenAI customers broaden the revenue base and reduce concentration.

Bear case:
- The >$20B OpenAI figure is over-capitalized before revenue and margin conversion are visible.
- OpenAI/G42 warrants and SBC dilute the per-share upside.
- Data-center/power/lease obligations consume more value than revenue multiples imply.
- Low float and post-IPO price discovery create a tradeability trap.

## CRWV Readiness Review

CRWV should be valued through enterprise value and an RPO-to-equity-FCF waterfall, not market cap / sales alone.

| Gate | Current evidence | Review |
|---|---|---|
| Revenue scale | Q1 revenue $2.078B, up from $982M YoY. | Scale is real and materially more modelable than CBRS. |
| Backlog/RPO | IR backlog $99.4B; SEC RPO $98.8B. | Strong demand signal, but not cash earnings. |
| RPO timing | 36% in 0-24 months, 39% in months 25-48, 25% in months 49-84. | This is the right starting point for valuation. Long-duration buckets need higher haircut. |
| Adjusted EBITDA | $1.157B Q1, 56% margin. | Good pre-capital-structure profitability, but not enough for equity value. |
| GAAP net loss | $740M Q1 net loss. | Confirms EBITDA does not yet translate to GAAP equity earnings. |
| Debt | $25.149B total debt principal; $7.547B current debt. | First-order valuation variable. Equity must be valued after debt service/refinancing risk. |
| Interest | Q1 net interest expense $536M; cash interest paid net of capitalized amounts $364M. | Interest can absorb a large share of EBITDA. |
| Capex/PP&E | Q1 PP&E purchases $7.695B; PP&E depreciation/amortization $1.1B. | The core risk is whether capex intensity normalizes before debt/depreciation consume the backlog economics. |
| Customer concentration | Customer A/B were 65% of Q1 revenue; named significant customers include OpenAI, Microsoft, Meta. | High-quality counterparties help, but concentration and renegotiation risk remain material. |

### CRWV Valuation Position

CRWV is **valuation-framework ready but not trade-memo ready**. The evidence is sufficient to build the first full model because the RPO maturity schedule, capex, debt, interest, EBITDA, and GAAP loss are already quantified. The missing piece is not another revenue multiple; it is the waterfall from RPO to equity cash earnings.

The required model should look like this:

| Step | Base mechanic | Key haircut / sensitivity |
|---|---|---|
| 1. RPO conversion | 0-24 month bucket ~$35.6B; 25-48 month bucket ~$38.5B; 49-84 month bucket ~$24.7B. | Haircut by duration, customer concentration, cancellation/credit terms, and delivery timing. |
| 2. Revenue to EBITDA | Apply utilization and adjusted EBITDA margin assumptions, starting from Q1 56%. | GPU cohort pricing, utilization, customer mix, power cost, renewal pricing. |
| 3. EBITDA to cash flow | Deduct cash interest, taxes, working capital, and lease/OEM financing effects. | Interest rate/refinancing path and capitalized interest treatment. |
| 4. Capex/depreciation | Deduct PP&E purchases and model economic asset consumption. | Growth vs maintenance capex, GPU useful life, obsolescence, residual value. |
| 5. EV to equity | Value on EV/revenue, EV/EBITDA, and DCF-style FCF, then subtract debt net of cash. | Debt maturities, refinancing spread, current debt, dilution from future equity/debt raises. |

### CRWV Mispricing Thesis

Bull case:
- Near-term RPO converts on schedule and validates a multi-year revenue ramp.
- Adjusted EBITDA margin stays near 50%+ as capacity utilization rises.
- Capex intensity declines after the largest buildout phase.
- Interest expense falls as a percentage of revenue/EBITDA and refinancing becomes less punitive.
- The market over-discounts leverage and underprices contracted AI compute demand.

Bear case:
- Backlog is over-capitalized even though conversion is multi-year and execution-heavy.
- Debt, interest, depreciation, and growth capex capture too much of the economics before equity holders.
- A major customer delays, renegotiates, or concentrates bargaining power.
- GPU obsolescence shortens economic useful life and raises maintenance capex.
- EV multiples compress once investors focus on equity FCF rather than backlog.

## Comparative Tradeability And Valuation Readiness

| Dimension | CBRS | CRWV |
|---|---|---|
| Primary edge | Newly public, low-coverage, direct OpenAI inference exposure. | Large disclosed backlog/RPO and visible AI infrastructure scale. |
| Main valuation blocker | Fully diluted cap table, warrant economics, OpenAI revenue schedule, float/liquidity. | RPO-to-FCF bridge, capex normalization, debt/interest/refinancing path. |
| Best valuation lens | Contracted revenue to gross profit to fully diluted per-share value. | EV and DCF-style RPO-to-equity-FCF waterfall. |
| Biggest false shortcut | Treating >$20B contract or $25.0B RPO as value. | Treating $99.4B backlog / $98.8B RPO as equity cash value. |
| Tradeability risk | Post-IPO float, lock-up, ADV, options/borrow unknown. | More modelable, but leverage and capital-markets sensitivity dominate. |
| Readiness score | Evidence-rich but not per-share valuation-ready. | Ready for first full valuation model; not yet ready for trade memo. |

## Required Before Any Trade Memo

For CBRS:
- Post-IPO basic and fully diluted share count.
- OpenAI, G42, AWS/customer warrant dilution and revenue amortization schedule.
- Pro forma cash, debt, revolver usage, lease obligations, and data-center commitments.
- OpenAI annual revenue schedule by tranche and acceptance criteria.
- Hardware vs cloud/services margin bridge.
- Float, lock-up schedule, ADV, options liquidity, and borrow availability.

For CRWV:
- Full EV bridge using current market cap, cash, debt, leases/OEM financing, and any new financing.
- RPO conversion by 0-24, 25-48, and 49-84 month buckets with customer and duration haircuts.
- Adjusted EBITDA to operating cash flow bridge.
- Cash interest, debt maturity, and refinancing schedule.
- PP&E purchases split between growth and maintenance capex.
- Depreciation/useful-life sensitivity by GPU cohort.
- Customer concentration and cancellation/renegotiation risk weights.

## Final Review

Tasks #31 and #32 are approved for synthesis with caveats.

CBRS should remain on the high-upside watchlist but should not be valued from headline contract/RPO metrics until dilution, warrant accounting, OpenAI revenue timing, lease/capex needs, and tradable float are solved. CRWV has enough hard data for a first full valuation model, but the model must be EV-based and must connect RPO conversion to equity FCF after capex, depreciation, debt, and interest.

The right manager headline is:

> CBRS is an information-edge candidate; CRWV is a backlog-quality and leverage-underwriting candidate. In both cases, the mispricing question is not "AI demand exists," but "how much of contracted demand becomes durable per-share cash value for equity holders."
