# OpenAI IPO / $1T Valuation Source Map & Data Dictionary

Date: 2026-06-28
Owner: @EvidenceAnalyst
Task: #all task #28, supporting #all task #27
Scope: evidence support only. Valuation conclusions are left to @ValuationReviewer.

## 1. Purpose

Build a clean evidence layer for OpenAI IPO / $500B, $850B, $1T valuation support tests.

The key rule is to avoid mixing:
- official funding valuation,
- reported operating metrics,
- rumored secondary-market marks,
- and public-market valuation equivalents.

## 2. Source Map

| Evidence bucket | Source | Label | What it supports | Caveat |
|---|---|---|---|---|
| Funding / valuation | OpenAI, "Scaling AI for everyone" https://openai.com/index/scaling-ai-for-everyone/ | confirmed | $110B new investment at $730B pre-money valuation; SoftBank $30B, NVIDIA $30B, Amazon $50B; Amazon partnership and NVIDIA inference compute. | Official funding valuation is a private valuation anchor, not public market price. |
| Funding / revenue / user scale | OpenAI, "Accelerating the next phase of AI" https://openai.com/index/accelerating-the-next-phase-ai/ | confirmed | $122B committed capital at $852B post-money valuation; more than 900M weekly active users; over 50M subscribers; $2B revenue/month; ads pilot >$100M ARR; growth history. | Official but still high-level; no audited financials, gross margin, burn, or segment P&L. |
| Enterprise / API scale | OpenAI, "The next phase of enterprise AI" https://openai.com/index/next-phase-of-enterprise-ai/ | confirmed | Enterprise >40% of revenue, on track to reach parity with consumer by end-2026; APIs process >15B tokens/min; Codex 3M WAU. | No enterprise ARR table, retention, gross margin, or customer concentration detail. |
| Consumer user scale | OpenAI funding posts; TechCrunch user milestone https://techcrunch.com/2026/02/27/chatgpt-reaches-900m-weekly-active-users/ | confirmed / reported | 900M+ weekly active users; 50M paying subscribers. | TechCrunch is secondary confirmation; official source preferred. Does not disclose churn or ARPU. |
| Annualized revenue cross-check | Reuters via Yahoo/MarketScreener: https://finance.yahoo.com/news/openai-tops-25-billion-annualized-033836274.html and https://www.marketscreener.com/news/openai-tops-25-billion-in-annualized-revenue-the-information-reports-ce7e5fdadf02c | reported | The Information reported OpenAI topped $25B annualized revenue by end-Feb 2026; Reuters could not verify. | Keep `reported`; do not treat as audited or company-disclosed. |
| Amazon partnership | OpenAI / Amazon partnership https://openai.com/index/amazon-partnership/ ; Amazon announcement https://www.aboutamazon.com/news/aws/amazon-open-ai-strategic-partnership-investment ; AWS roundup https://aws.amazon.com/blogs/aws/aws-weekly-roundup-openai-partnership-aws-elemental-inference-strands-labs-and-more-march-2-2026/ | confirmed | Amazon investment/partnership; OpenAI Frontier on AWS; OpenAI to consume Trainium capacity; Amazon investment timing/conditions; 2GW Trainium and expanded AWS agreement details from Amazon. | Need separate investment economics vs compute purchase obligations. |
| NVIDIA partnership | OpenAI/NVIDIA systems partnership https://openai.com/index/openai-nvidia-systems-partnership/ ; NVIDIA release https://nvidianews.nvidia.com/news/openai-and-nvidia-announce-strategic-partnership-to-deploy-10gw-of-nvidia-systems | confirmed | At least 10GW NVIDIA systems; first GW targeted second half 2026 on Vera Rubin; NVIDIA may invest progressively as deployment milestones are met. | Partnership capacity is not revenue; timing, cost, and financing terms need tracking. |
| Microsoft relationship | Microsoft/OpenAI continuing partnership statement https://blogs.microsoft.com/blog/2026/02/27/microsoft-and-openai-joint-statement-on-continuing-partnership/ ; Microsoft/OpenAI next chapter https://blogs.microsoft.com/blog/2025/10/28/the-next-chapter-of-the-microsoft-openai-partnership/ | confirmed | Microsoft IP relationship continues unchanged; Microsoft had 32.5% as-converted stake excluding later rounds; Amazon partnership contemplated under agreements. | Need updated ownership after 2026 funding; OpenAI profit share / revenue share not fully visible. |
| OpenAI custom compute | OpenAI / Broadcom Jalapeño page https://openai.com/index/openai-broadcom-jalapeno-inference-chip/ ; OpenAI / Broadcom strategic collaboration https://openai.com/index/openai-and-broadcom-announce-strategic-collaboration/ ; Axios report https://www.axios.com/2026/06/24/openai-jalapeno-ai-chip-broadcom-nvidia ; The Verge report https://www.theverge.com/ai-artificial-intelligence/955939/openai-reveals-its-first-ai-processor-jalapeno | confirmed / reported | Jalapeño inference chip with Broadcom; 10GW OpenAI-designed accelerator collaboration; potential inference cost and Nvidia dependency mitigation. | Use OpenAI pages for confirmed chip/collaboration facts; media claims on performance/cost need `reported`. |
| Secondary / rumored valuation | Private-market reports, secondary-market chatter, social posts | rumored unless named transaction/source | Possible valuation path toward $850B / $1T. | Do not use as valuation base without named source and terms. |

## 3. Data Dictionary

| Field | Label default | Definition | How to use in valuation support |
|---|---|---|---|
| latest_official_funding_valuation | confirmed | Official pre-money / post-money valuation from OpenAI funding announcements. Current official anchors: $730B pre-money from the $110B announcement and $852B post-money from the later $122B committed-capital close. | Valuation anchor; compare to $500B / $850B / $1T scenarios. |
| funding_amount_by_investor | confirmed | Stated investment amounts by SoftBank, NVIDIA, Amazon, and later investors where official. | Helps separate strategic capital from financial investor demand. |
| annualized_revenue | reported unless official | ARR / annualized revenue estimate from Reuters/The Information or company statement. | Primary input to revenue multiple sanity check. |
| monthly_revenue | confirmed if from OpenAI | OpenAI says it is generating $2B revenue/month. | Annualize to $24B run-rate, but note absence of audited statements. |
| revenue_mix_consumer_enterprise_api | confirmed / missing | Consumer subscriptions, enterprise, API, ads, and other revenue split. | Needed for durability and margin model. |
| enterprise_revenue_share | confirmed | OpenAI says enterprise is >40% of revenue and on track to parity with consumer by end-2026. | Supports enterprise durability thesis; still needs retention/margin detail. |
| weekly_active_users | confirmed | ChatGPT weekly active users. | Top-of-funnel scale; not valuation support unless linked to monetization. |
| paying_subscribers | confirmed | Consumer subscriber count. | Estimate consumer subscription revenue only if ARPU assumptions are explicit. |
| API_tokens_per_minute | confirmed | API traffic volume. | Usage growth proxy; needs pricing and cost to become economics. |
| Codex_WAU | confirmed | Codex weekly active users. | Agentic/workflow adoption proxy. |
| gross_margin | missing | Gross margin by consumer/API/enterprise/ads. | Critical for $1T valuation support; must be estimated with scenario ranges. |
| inference_cost_per_unit | missing / reported | Cost to serve tokens or queries. | Main bridge between usage scale and FCF. |
| compute_commitments | confirmed / reported | AWS Trainium, NVIDIA systems, other compute agreements. | Capex/COGS pressure and L1 pass-through mapping. |
| cloud_partner_economics | missing | Revenue share, discounts, take-or-pay, compute financing, and capacity guarantees. | Needed to judge OpenAI FCF and partner upside for MSFT/AMZN/NVDA/ORCL/CRWV. |
| burn_or_operating_loss | missing / reported | Operating loss, R&D, infrastructure losses. | Required for IPO readiness and FCF margin path. |
| governance_listing_path | confirmed / reported | Board/control, nonprofit/PBC structure, MOU/partnership constraints, IPO comments. | Determines IPO probability and public-market discount. |
| related_party_or_partner_dependency | confirmed / missing | Microsoft/Amazon/NVIDIA/SoftBank economic dependencies. | Determines whether value accrues to OpenAI or public L1 suppliers/partners. |

## 4. Evidence Labels for Current Key Inputs

| Input | Current label | Use / do not use |
|---|---|---|
| $730B pre-money valuation from $110B round | confirmed | Use as official private valuation anchor. Do not call it market cap. |
| $122B committed capital at $852B post-money and $2B/month revenue | confirmed | Use as latest official private valuation / operating scale anchor; still unaudited. |
| $25B annualized revenue from The Information / Reuters | reported | Use as cross-check only; not official. |
| 900M+ WAU and 50M+ subscribers | confirmed | Use as scale/monetization funnel evidence. |
| Enterprise >40% of revenue | confirmed | Use as mix evidence, but not segment P&L. |
| API >15B tokens/min | confirmed | Use as developer/API usage proxy, not revenue proxy without price/cost assumptions. |
| Amazon 2GW Trainium / AWS expansion | confirmed | Use as compute capacity / partner mapping evidence. |
| NVIDIA 10GW systems | confirmed | Use as compute commitment / L1 mapping evidence. |
| Microsoft ownership stake / IP continuity | confirmed for cited statements | Use for partner exposure, but update ownership after latest round is missing. |
| $850B or $1T valuation | reported / scenario | Treat as valuation scenario unless tied to confirmed transaction terms. |

## 5. Models / Theory for Valuation Support

### A. Revenue Multiple Sanity Check

Purpose: translate $500B / $850B / $1T valuation into required revenue scale.

Required inputs:
- current official run-rate revenue,
- reported ARR cross-check,
- 2030 revenue scenario,
- public comparable multiple set: MSFT, GOOGL, AMZN/AWS proxy, ORCL, PLTR, SNOW, CRM, high-growth software/infrastructure comps.

Output:
- implied EV/revenue at current run-rate,
- required 2030 revenue at 10x / 15x / 20x / 25x revenue,
- what growth CAGR is needed from current run-rate.

### B. FCF / DCF Support Test

Purpose: test whether $1T can be supported by cash generation, not just revenue.

Required inputs:
- 2030 revenue,
- gross margin,
- R&D / SG&A as % revenue,
- compute/capex intensity,
- FCF margin,
- terminal multiple or discount-rate assumptions.

Key sensitivity:
- 20% vs 30% vs 40% long-run FCF margin.
- inference cost decline.
- cloud partner gross margin leakage.

### C. Platform Option Value Model

Purpose: capture non-linear upside if OpenAI becomes a platform, not just a model vendor.

Components:
- consumer super-app,
- enterprise AI operating layer,
- API/developer platform,
- agent workflow ecosystem,
- ads/search/discovery monetization,
- possible app-store/revenue-share layer.

Data needed:
- retention,
- paid conversion,
- enterprise net revenue retention,
- developer/API growth,
- app/agent ecosystem economics.

### D. Value-Chain Pass-Through Model

Purpose: decide whether OpenAI value is already captured by public L1 names.

Map OpenAI scaling to:
- MSFT: IP rights, Azure/API hosting, enterprise distribution, ownership economics.
- AMZN: AWS/Trainium/Frontier distribution and strategic investment.
- NVDA: 10GW systems and GPU demand.
- AVGO / TSM: custom/inference silicon and advanced node demand.
- ORCL / CRWV: potential AI cloud capacity / RPO / GPU cloud demand.
- GOOGL: competitive cloud/model impact, Anthropic comparison.

Output:
- if OpenAI is not directly investable, which public names capture the economics and where expectations may be wrong.

## 6. Immediate Cleaning Checklist

Before @ValuationReviewer uses any number:
1. Mark every revenue number as official / reported / rumored.
2. Separate revenue, ARR, monthly run-rate, and booking/backlog language.
3. Separate funding valuation from secondary valuation and IPO scenario valuation.
4. Separate compute commitments from capex, COGS, and revenue.
5. Identify whether partner economics accrue to OpenAI or L1 public partners.
6. Keep burn/profitability as missing unless sourced from a credible report.

## 7. Current Critical Data Gaps

- audited revenue and revenue by segment.
- gross margin by consumer subscription, API, enterprise, ads.
- inference cost per token / per query.
- R&D, sales/marketing, and infrastructure burn.
- capex and committed compute obligations.
- Microsoft/Amazon/NVIDIA/SoftBank ownership and economics after the latest round.
- customer retention, enterprise NRR, API customer concentration.
- IPO timing, governance, and public-company structure.
