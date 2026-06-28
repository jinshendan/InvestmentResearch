# OpenAI L1 Pass-Through Valuation Review

**Date:** 2026-06-28  
**Owner:** @ValuationReviewer  
**Task:** #37 review of task #33 OpenAI L1 pass-through matrix  
**Reviewed artifacts:**  
- `reports/openai_l1_pass_through_matrix_task33_2026-06-28.md`  
- `reports/openai_ipo_source_map_data_dictionary_task28_2026-06-28.md`  
- `reports/valuation/openai_ipo_valuation_support_model_2026-06-28.md`

## Verdict

Task #33 is usable for manager synthesis. The matrix gets the most important valuation rule right: OpenAI's private valuation, revenue run-rate, compute commitments, cloud spend, supplier revenue, strategic investment dollars, and RPO/backlog are separate economics and must not be double-counted.

The pass-through ranking is directionally sound:

- **Highest-quality positive pass-through:** AMZN, MSFT, NVDA, AVGO.
- **Direct but capex/financing-sensitive pass-through:** ORCL.
- **Direct but small-cap / dilution / contract-conversion-sensitive pass-through:** CBRS.
- **Backlog-quality and leverage-sensitive pass-through:** CRWV.
- **Second-order supply-chain pass-through:** TSM.
- **Ambiguous competitive pass-through:** GOOGL.

For public-stock valuation, the task #33 matrix should be treated as an exposure map and risk framework, not as a buy list. The next step is to assign each public name a probability-weighted revenue, margin, capex, and FCF effect before translating OpenAI exposure into stock value.

## Source Spot Check

I spot-checked the key official source logic against the task #33 source set:

| Source area | Valuation relevance |
|---|---|
| OpenAI official funding update: $122B committed capital at $852B post-money and $2B/month revenue. | Supports OpenAI valuation/run-rate anchor, but not supplier revenue or public-stock upside by itself. |
| Microsoft/OpenAI agreement update: Microsoft stake, IP rights, Azure API exclusivity, $250B Azure purchase commitment, loss of compute ROFR. | Supports direct MSFT exposure, but also confirms multi-cloud leakage risk. |
| OpenAI/Amazon partnership: $50B Amazon investment, AWS Frontier distribution, 2GW Trainium, expanded AWS agreement. | Supports AMZN as one of the cleanest confirmed pass-through names, but investment return and AWS operating profit must be separated. |
| OpenAI/NVIDIA systems partnership: at least 10GW NVIDIA systems and up to $100B progressive NVIDIA investment tied to GW deployment. | Supports NVDA demand, but introduces circular-financing and LOI-to-revenue timing risk. |
| OpenAI/Broadcom collaboration: 10GW custom accelerators and Broadcom Ethernet/connectivity systems, targeted deployment from H2 2026 through 2029. | Supports AVGO custom silicon/networking exposure, but revenue per GW and margin are not disclosed. |

## Public-Stock Valuation Impact

| Public name | Valuation impact from OpenAI | What can be used now | What cannot be used yet |
|---|---|---|---|
| MSFT | Direct ownership/IP/Azure/API economics make MSFT the broadest OpenAI-linked public platform exposure. | Use as positive Azure/Copilot/platform option evidence. | Do not value MSFT by multiplying OpenAI's private valuation by stake without updated ownership, revenue-share, tax, dilution, and holding-company treatment. |
| AMZN | Clean direct positive exposure through AWS distribution, Trainium capacity, and strategic investment. | Use as evidence that AWS has a credible OpenAI workload path and Trainium validation. | Do not count the $50B investment as AWS revenue; do not assume Trainium margin without capacity pricing and utilization. |
| NVDA | Large OpenAI systems roadmap validates continued frontier GPU demand. | Use as demand-duration support for accelerator/networking cycles. | Do not treat 10GW capacity or up to $100B investment as immediate NVIDIA revenue; adjust for LOI timing, supplier financing, and custom-silicon substitution. |
| AVGO | OpenAI custom accelerator and Ethernet route gives AVGO differentiated pass-through. | Use as custom-silicon/networking upside evidence. | Do not assume OpenAI custom chip demand is incremental to NVIDIA without workload split and production economics. |
| ORCL | Stargate/OCI capacity can create large AI cloud revenue. | Use as direct AI infrastructure exposure. | Do not capitalize headline capacity before capex funding, power, debt, revenue recognition, and OCI margin are known. |
| CBRS | Very direct OpenAI inference exposure gives high upside if tranches convert. | Use as an information-edge candidate and contract-conversion watch item. | Do not use >$20B contract or $25.0B RPO as equity value; dilution, warrants, contra-revenue, lease/capex, and float block valuation. |
| CRWV | OpenAI and frontier-lab workloads support demand, but equity value is a debt/capex problem. | Use as backlog-quality and utilization sensitivity evidence. | Do not attribute all $99.4B backlog / $98.8B RPO to OpenAI or treat RPO as FCF. |
| TSM | Likely second-order beneficiary if NVIDIA/custom accelerator demand pulls advanced nodes/packaging. | Use as supply-chain sensitivity, not direct contract exposure. | Do not underwrite OpenAI-specific TSM revenue without foundry/package allocation disclosure. |
| GOOGL | OpenAI can be a cloud customer but is also a competitive threat to Gemini/Search. | Use as an ambiguous read-through: possible GCP upside, platform/search pressure. | Do not treat OpenAI growth as automatically positive for GOOGL without Google Cloud contract economics and competitive impact. |

## Double-Counting Risk Map

The highest-risk mistakes are:

| Mistake | Correct treatment |
|---|---|
| Add OpenAI's $852B post-money valuation to MSFT/AMZN/NVDA market value. | Private valuation is an OpenAI capital anchor; public partner value depends on ownership economics or operating profit capture. |
| Treat OpenAI's $2B/month revenue as cloud or supplier revenue. | OpenAI revenue is customer revenue; partner revenue depends on cloud, hardware, licensing, or revenue-share contracts. |
| Treat Amazon/NVIDIA investment dollars as supplier revenue. | Strategic investment is capital deployed into OpenAI; it may support future purchases but is not the same as revenue. |
| Treat 10GW / 2GW / 750MW capacity as revenue. | Capacity needs price, timing, utilization, acceptance, margin, capex, and financing to become valuation. |
| Attribute all CRWV backlog/RPO to OpenAI. | Only OpenAI-specific contracts should be mapped to OpenAI; total RPO includes other customers and timing buckets. |
| Treat CBRS RPO or OpenAI deal value as equity upside before dilution. | Customer warrants, warrant amortization, SBC, post-IPO shares, and float/liquidity can change per-share value materially. |
| Count the same OpenAI workload through MSFT, ORCL, CRWV, AMZN, NVDA, AVGO, and TSM at 100% each. | Build a value-chain map: one OpenAI workload can create revenue for multiple suppliers, but each captures only its own margin pool. |

## Valuation Weighting By Name

For manager synthesis, I would weight the evidence as follows:

| Name | Valuation weight | Reason |
|---|---|---|
| AMZN | High positive, needs margin proof | Official strategic investment, AWS distribution, Trainium capacity, and expanded agreement make the evidence clean. The valuation issue is AWS revenue timing and margin. |
| MSFT | High positive, but partially mature/known | Strongest long-term relationship and ownership/IP economics, but multi-cloud shift and loss of compute ROFR reduce exclusivity. |
| NVDA | High positive, high expectation risk | OpenAI supports demand duration, but the stock may already discount broad AI accelerator demand; custom silicon and Trainium cap upside. |
| AVGO | Medium-high positive | Direct OpenAI custom silicon/networking validation; economics are less visible than the headline capacity. |
| ORCL | Medium positive / high execution risk | Large infrastructure path, but public-stock upside depends on OCI margin, capex funding, and debt/power execution. |
| CBRS | High option value / high blocker risk | Direct OpenAI exposure could be mispriced, but valuation is blocked by dilution, warrant amortization, contract timing, and liquidity. |
| CRWV | Medium demand signal / high equity-FCF risk | Demand is real, but debt, interest, depreciation, PP&E, and customer concentration determine equity value. |
| TSM | Medium-low direct weight | Likely beneficiary of the AI supply chain, but OpenAI-specific evidence is inferred. |
| GOOGL | Ambiguous | OpenAI may be a cloud customer, but OpenAI's success may also pressure Google AI/search economics. |

## Manager Synthesis Rules

Use task #33 for:
- Exposure taxonomy across equity, cloud, GPU, custom silicon, data center, backlog, and competitive pressure.
- Source-quality ranking of confirmed direct vs inferred exposure.
- Identifying which public names need valuation work next.
- Double-counting controls for OpenAI private valuation and supplier economics.

Do not use task #33 for:
- Direct buy/sell ratings.
- Numeric per-share valuation impact.
- Public-market position sizing.
- Treating OpenAI commitments as fully contracted, fully margin-accretive public-company revenue.

## Required Before Trade Memo

Before OpenAI pass-through can become a trade memo, collect for each L1 name:

- Current adjusted close / market cap / EV / share count.
- Consensus revenue, EBITDA, FCF, and capex for 2026-2028.
- OpenAI-specific revenue recognition schedule where disclosed.
- Gross margin and incremental operating margin on OpenAI workloads.
- Capex, working capital, debt, or strategic investment funding burden.
- Customer concentration, termination, cancellation, or renegotiation clauses.
- Probability weights for confirmed contract, announced capacity, LOI, inferred supply chain, and competitive pressure.

## Final Review

Task #33 is approved for synthesis with caveats.

The best manager headline is:

> OpenAI pass-through is investable only after separating ownership value, cloud revenue, hardware revenue, strategic investment, compute capacity, RPO/backlog, and competitive pressure. The cleanest positive public exposures are AMZN/MSFT/NVDA/AVGO, but the highest mispricing candidates may be CBRS and CRWV because the market can misread headline contracts/backlog before dilution, capex, interest, and FCF are solved.
