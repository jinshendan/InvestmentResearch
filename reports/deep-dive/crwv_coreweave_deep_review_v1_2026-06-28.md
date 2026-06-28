# CRWV / CoreWeave Deep Review v1

Date: 2026-06-28
Owner: @SemisAIInfraEvidenceScout
Task: #24

## Mispricing Thesis To Prove Or Disprove

CRWV may be mispriced because investors can interpret the $99B backlog/RPO in two opposite ways. The bull case is that CoreWeave has locked in scarce AI compute demand and can convert backlog into high EBITDA as power/GPU capacity comes online. The bear case is that backlog is not "cash in the bank": conversion depends on customer credit, delivery timing, GPU depreciation, power/data-center execution, and expensive debt-funded capex.

## Confirmed Evidence

| Item | Confirmed data | Evidence label | Source |
| --- | --- | --- | --- |
| Public status | Nasdaq listing completed in March 2025. | confirmed | IR release: https://investors.coreweave.com/news/news-details/2026/CoreWeave-Reports-Strong-First-Quarter-2026-Results/ |
| Q1 revenue | Revenue $2.078B vs $982M YoY. | confirmed | IR release |
| Profitability | Operating loss $144M; net loss $740M; adjusted EBITDA $1.157B, 56% margin; adjusted net loss $589M. | confirmed | IR release |
| Revenue backlog | Company press release states revenue backlog $99.4B as of March 31, 2026. SEC 10-Q discloses unsatisfied RPO $98.8B. | confirmed | IR release; SEC 10-Q: https://www.sec.gov/Archives/edgar/data/1769628/000176962826000222/crwv-20260331.htm |
| RPO timing | 36% of RPO expected over 24 months ending Mar. 31, 2028; 39% months 25-48; remaining balance months 49-84. | confirmed | SEC 10-Q |
| Revenue model | 98% of Q1 revenue related to customer commitments, including capacity delivered before commitment start dates. | confirmed | SEC 10-Q |
| Customer concentration | Q1 revenue: Customer A 45%, Customer B 20%. Accounts receivable: Customer A 39%, B 17%, C 22%. | confirmed | SEC 10-Q |
| Named customer exposure | Risk factor names OpenAI contract up to about $11.9B through Oct. 2030; other significant customers include Microsoft and Meta. | confirmed | SEC 10-Q |
| New wins | Meta $21B commitment; Anthropic multi-year agreement; expanded Cohere, Jane Street, Mistral relationships. | confirmed | IR release |
| Power scale | Surpassed 1GW active power; contracted power above 3.5GW; target path to >8GW by 2030. | confirmed / target for 2030 | IR release |
| Debt | Total debt principal $25.149B; debt net of discounts/costs $24.859B; current debt $7.547B. | confirmed | SEC 10-Q |
| Interest expense | Q1 interest expense, net $536M; contractual interest expense $483M; cash interest paid net of capitalized amounts $364M. | confirmed | IR release; SEC 10-Q |
| Capex / fixed assets | Purchase of property and equipment $7.695B in Q1; property and equipment net $36.424B; depreciation/amortization on property and equipment $1.1B. | confirmed | SEC 10-Q |
| Market data | Current price $96.58; market cap about $50.9B; latest trade timestamp June 27, 2026 00:15 UTC. | market data snapshot | OpenAI finance tool snapshot |

## Backlog Quality Bridge

| Question | Evidence so far | Interpretation |
| --- | --- | --- |
| Is the headline backlog real? | IR says $99.4B revenue backlog; SEC says $98.8B RPO under GAAP revenue note. | Yes as disclosed commitments/RPO, but not equivalent to guaranteed cash or near-term revenue. |
| How fast can it convert? | 36% of RPO over first 24 months; 39% months 25-48; balance months 49-84. | Conversion is multi-year and delivery-constrained. A large part is long-duration infrastructure execution, not immediate revenue. |
| Who underwrites it? | Customer A/B are 65% of revenue; named significant customers include OpenAI, Microsoft, Meta. | Customer concentration is central. Backlog quality depends on counterparty quality and customer AI economics. |
| What does conversion cost? | Q1 PP&E purchases $7.7B; debt principal $25.1B; Q1 interest expense net $536M; PP&E depreciation/amortization $1.1B. | Backlog has heavy financing and depreciation load. Need FCF conversion, not just EBITDA. |
| Is the model profitable? | Adjusted EBITDA 56% margin, but GAAP net loss $740M. | EBITDA is strong before debt/depreciation. Equity value depends on whether scale lowers cost of capital faster than depreciation/interest consume economics. |

## First-Pass Valuation Sanity

| Metric | Calculation | Read-through |
| --- | --- | --- |
| Market cap / run-rate revenue | $50.9B / ($2.078B * 4) = about 6.1x | Not obviously extreme if revenue doubles, but assumes backlog converts. |
| Enterprise value estimate | $50.9B market cap + $24.9B debt - $3.34B cash/restricted cash/marketable securities = about $72.4B | EV is much higher than equity market cap due to debt-funded buildout. |
| EV / run-rate revenue | $72.4B / $8.312B = about 8.7x | The real valuation lens should use EV, not just market cap. |
| EV / run-rate adjusted EBITDA | $72.4B / ($1.157B * 4) = about 15.6x | Reasonable only if adjusted EBITDA converts to durable FCF after capex and interest normalize. |
| Interest burden | Q1 net interest expense $536M / revenue $2.078B = about 26% of revenue | Debt cost is a first-order thesis variable. |
| Capex intensity | Q1 PP&E purchases $7.695B / revenue $2.078B = about 3.7x quarterly revenue | Growth is deeply capital-intensive. |

## What Must Be Proven For Long Thesis

1. RPO converts on schedule without material cancellations, credits, or delivery delays.
2. OpenAI/Microsoft/Meta and other large customers remain creditworthy and expand usage.
3. Next-gen GPU deployments lift utilization and price without reducing useful life assumptions.
4. Cost of capital declines after scale, reducing the drag from 9%-15% debt.
5. Adjusted EBITDA begins converting to operating cash flow and then FCF after capex moderation.

## What Would Break The Thesis

1. Backlog additions slow while capex and debt obligations stay elevated.
2. Customer concentration remains high and one major customer delays or renegotiates.
3. Depreciation/technology obsolescence accelerates as GPU generations roll.
4. Power/data-center constraints push RPO conversion rightward.
5. Equity investors price only revenue growth while debt holders capture the economics.

## Data Gaps

- Customer-by-customer backlog/RPO maturity, credit protection, and cancellation/credit clauses.
- GPU generation mix and useful-life/depreciation assumptions by cohort.
- Maintenance capex vs growth capex.
- Power contract cost curve and data-center lease obligations by region.
- Unit economics by customer type: AI lab, hyperscaler, enterprise, inference vs training.
- Detailed FCF bridge from adjusted EBITDA to cash after interest, PP&E, leases, and OEM financing.

## Tracking Metrics

- RPO/backlog additions, conversion, and % expected within 24 months.
- Revenue concentration and AR/customer concentration.
- Active power, contracted power, and datacenter delivery milestones.
- PP&E purchases, capitalized interest, and debt drawdown.
- Interest expense as % of revenue and adjusted EBITDA coverage.
- Depreciation/amortization per GPU/asset cohort.
- Operating cash flow, FCF after capex, and lease/OEM financing obligations.

## Initial View

CRWV is a better "backlog-quality" trade than a simple AI demand trade. The key question is not whether $99B was disclosed; it was. The question is how much of that RPO becomes cash earnings for equity after customer concentration, delivery risk, depreciation, and debt service. First deep-dive priority should be an RPO conversion waterfall plus capex/debt/interest burden model.

