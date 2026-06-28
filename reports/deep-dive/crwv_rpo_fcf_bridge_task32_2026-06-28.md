# CRWV Follow-Up: RPO Conversion Waterfall + Capex/Debt/Interest/FCF Bridge

Date: 2026-06-28
Owner: @SemisAIInfraEvidenceScout
Task: #32

## Purpose

CRWV's $99.4B revenue backlog / $98.8B RPO is real as a disclosed metric, but it is not the same as equity cash earnings. This bridge converts backlog into time buckets and then deducts the operating, capex, depreciation, interest, and financing burdens that determine how much value accrues to equity.

Primary sources:
- Q1 2026 results: https://investors.coreweave.com/news/news-details/2026/CoreWeave-Reports-Strong-First-Quarter-2026-Results/
- Q1 2026 10-Q: https://www.sec.gov/Archives/edgar/data/1769628/000176962826000222/crwv-20260331.htm

## Confirmed Starting Point

| Area | Confirmed item | Why it matters |
| --- | --- | --- |
| Q1 revenue | $2.078B vs $982M YoY. | Base revenue scale. |
| Adjusted EBITDA | $1.157B, 56% adjusted EBITDA margin. | Strong pre-capex/debt profitability measure. |
| GAAP net loss | $740M. | Equity economics are not captured by adjusted EBITDA alone. |
| Revenue backlog / RPO | IR revenue backlog $99.4B; SEC unsatisfied RPO $98.8B. | Core investment debate. |
| RPO timing | 36% expected over 0-24 months; 39% over months 25-48; remaining 25% over months 49-84. | Converts headline backlog into duration and execution risk. |
| Customer concentration | Q1 revenue: Customer A 45%, Customer B 20%; AR: Customer A 39%, B 17%, C 22%. | Backlog quality depends on few large customers. |
| Named customer exposure | Risk factor names OpenAI contract up to about $11.9B through Oct. 2030; other significant customers include Microsoft and Meta. | Counterparty and bargaining-power risk. |
| New commitments | Meta $21B commitment; Anthropic multi-year agreement; expanded Cohere, Jane Street, Mistral. | Backlog additions tied to AI labs/hyperscalers. |
| Power scale | >1GW active power; >3.5GW contracted power; target >8GW by 2030. | Delivery capacity is physical infrastructure-constrained. |
| Debt | Total debt principal $25.149B; debt net of discounts/costs $24.859B; current debt $7.547B. | Interest and refinancing are first-order equity variables. |
| Interest | Q1 interest expense net $536M; contractual interest expense $483M; cash interest paid net of capitalized amounts $364M. | Debt burden can absorb EBITDA. |
| Capex / PP&E | Q1 PP&E purchases $7.695B; PP&E net $36.424B; PP&E depreciation/amortization $1.1B. | RPO conversion requires heavy upfront capital and depreciation. |

## RPO Conversion Waterfall

Using SEC RPO of $98.8B:

| Conversion bucket | % of RPO | Dollar amount | Annualized rough revenue run-rate if recognized evenly | Key risk |
| --- | ---: | ---: | ---: | --- |
| 0-24 months | 36% | ~$35.6B | ~$17.8B/year | Near-term delivery, power, GPU supply, customer acceptance. |
| Months 25-48 | 39% | ~$38.5B | ~$19.3B/year | Customer AI economics and contract durability over 2-4 years. |
| Months 49-84 | 25% | ~$24.7B | ~$7.1B/year over 3 years | Highest discount for technology obsolescence and renegotiation risk. |
| Total | 100% | ~$98.8B | n/a | Not all backlog is equal-duration or equal-quality. |

Using IR backlog of $99.4B gives nearly the same split: ~$35.8B, ~$38.8B, and ~$24.9B.

## From Backlog To Equity Cash Earnings

| Step | Formula | Current anchor / issue |
| --- | --- | --- |
| 1. RPO conversion | Recognized revenue by bucket = RPO bucket * conversion rate * non-cancellation factor. | Start with SEC timing; haircut long-duration buckets. |
| 2. Gross / EBITDA conversion | Adjusted EBITDA = revenue * adjusted EBITDA margin. | Q1 adjusted EBITDA margin 56%, but may vary by customer/GPU cohort. |
| 3. Interest burden | Pre-tax cash flow before capex = adjusted EBITDA - cash interest. | Q1 net interest expense $536M; cash interest paid net $364M. |
| 4. Maintenance / growth capex | FCF before financing = operating cash flow - PP&E purchases - leases/OEM financing. | Q1 PP&E purchases $7.695B vs revenue $2.078B. |
| 5. Depreciation / obsolescence | Economic earnings = revenue - opex - interest - true asset consumption. | Q1 PP&E depreciation/amortization $1.1B. |
| 6. Equity value | Equity cash earnings after debt service and reinvestment. | Debt principal $25.149B; use EV, not market cap only. |

## Q1 Bridge Snapshot

| Metric | Q1 figure | Ratio to revenue | Read-through |
| --- | ---: | ---: | --- |
| Revenue | $2.078B | 100% | Base. |
| Adjusted EBITDA | $1.157B | 56% | Strong infrastructure EBITDA before capital structure. |
| GAAP net loss | -$740M | -36% | Accounting/debt/depreciation burden still material. |
| Net interest expense | $536M | 26% | Large claim ahead of equity. |
| PP&E purchases | $7.695B | 370% | Growth consumes large capital. |
| PP&E depreciation/amortization | $1.1B | 53% | Asset consumption is economically important. |
| Total debt principal | $25.149B | 12.1x quarterly revenue | Capital structure dominates equity risk. |

## Backlog Quality Scoring

| Dimension | Current evidence | Score direction |
| --- | --- | --- |
| Counterparty quality | OpenAI, Microsoft, Meta named as significant customers / counterparties; new Meta and Anthropic commitments. | Positive credit-quality signal, but concentration risk remains. |
| Customer concentration | Customer A/B 65% of Q1 revenue; AR also concentrated. | Negative / requires customer-level risk monitoring. |
| Conversion timing | 75% of RPO expected within 48 months; 25% beyond 48 months. | Positive for visibility, but still long-duration. |
| Capacity readiness | >1GW active, >3.5GW contracted power. | Positive, but delivery and power execution still key. |
| Financing burden | $25.149B debt principal; Q1 net interest $536M. | Major negative for equity FCF. |
| Capex intensity | Q1 PP&E purchases $7.695B. | Major negative until growth capex normalizes. |
| Accounting quality | Adjusted EBITDA strong, GAAP net loss large. | Requires FCF bridge before valuation. |

## Scenarios

| Scenario | RPO conversion | EBITDA / capex / interest outcome | Equity implication |
| --- | --- | --- | --- |
| Bull | 0-24 month bucket converts on schedule; 25-48 month bucket renewed/expanded; long-duration contracts not renegotiated. | EBITDA margin stays near 50%+ while interest burden declines as % revenue and capex intensity moderates. | Backlog supports premium EV/revenue and EV/EBITDA. |
| Base | Near-term RPO converts, but capex and interest remain high; FCF lags EBITDA. | Revenue growth strong but equity cash earnings delayed. | Stock trades on execution milestones, not headline backlog. |
| Bear | Conversion slips, customer concentration persists, or contracts require concessions. | Debt/interest/depreciation consume EBITDA; capital markets risk rises. | Backlog was over-capitalized and equity multiple compresses. |

## Valuation Inputs For Next Pass

| Input | Base source | Needed for valuation |
| --- | --- | --- |
| Current share price / market cap | Market data refresh. | Equity value. |
| Debt net of cash | 10-Q plus latest financing. | Enterprise value. |
| RPO by maturity | SEC 10-Q percentages. | Revenue forecast. |
| Adjusted EBITDA margin | Q1 actual and guidance if available. | EBITDA forecast. |
| Cash interest | 10-Q / IR. | FCF bridge. |
| PP&E purchases / lease obligations | 10-Q cash flow and commitments. | Capex burden. |
| Depreciation by asset cohort | 10-Q; future filings. | Economic earnings and useful-life sensitivity. |
| Customer concentration | 10-Q. | Risk discount / scenario weights. |

## Decision Gate Before Valuation

CRWV can move to valuation only after the model explicitly shows:

1. RPO waterfall by 0-24, 25-48, and 49-84 month buckets.
2. Customer concentration haircut / scenario weights.
3. Adjusted EBITDA to operating cash flow bridge.
4. Interest and debt maturity schedule.
5. Growth capex vs maintenance capex split.
6. Depreciation/useful-life sensitivity for GPU cohorts.
7. EV-based multiples, not market-cap-only multiples.

## Initial Model Recommendation

Use an EV/revenue and EV/adjusted EBITDA framework only as a first screen. The investment conclusion should come from a DCF-style RPO conversion model where the main sensitivities are:

- RPO conversion rate and timing.
- EBITDA margin under utilization/price pressure.
- Capex intensity decline path.
- Interest expense / refinancing cost.
- GPU useful life and depreciation.
- Customer concentration haircut.

The correct framing is: "$99.4B backlog is a strong demand signal, but equity value depends on what remains after delivery cost, asset depreciation, and debt service."

