# AI/Tech Watchlist Valuation Framework v1

**Date:** 2026-06-27  
**Owner:** @ValuationReviewer  
**Parent watchlist:** `reports/ai_tech_target_watchlist_v1_canonical_2026-06-27.md`  
**Task:** Watchlist v1 valuation framework review: priority, valuation lenses, and mispricing criteria by company  

## Purpose

This framework converts the canonical AI/tech target universe into a valuation workflow. It is not a final investment conclusion. It defines what each company must prove for the current or reported valuation to be justified, where mispricing could exist, and which valuation lens should be used first.

## Global Review Rules

1. Start with market-implied expectations, not narrative.
2. Separate current fundamentals from long-duration AI/platform option value.
3. For public companies, use adjusted close / 前复权 price convention when price history matters.
4. For private companies, label valuation sources as disclosed, reported, secondary-market, or rumored.
5. Do not compare private-company valuation directly with public market cap without liquidity, disclosure, and capital-structure caveats.
6. Every review must include upside catalysts, downside catalysts, evidence gaps, and tracking data.

## Valuation Lenses

- **AI infrastructure compounder:** Revenue growth, gross margin durability, capex cycle, customer concentration, supply-chain bottlenecks, FCF conversion.
- **Platform monetization:** Installed base, distribution control, AI attach rate, ARPU/seat expansion, operating leverage.
- **Option-value battleground:** Current business value plus probability-weighted autonomy, robotics, AI agent, or platform optionality.
- **Semiconductor cycle / scarcity:** Capacity, advanced packaging, HBM/EUV exposure, cycle risk, geopolitical constraints.
- **Enterprise AI software:** Net retention, AI product attach, workflow depth, seat risk, competitive bundling.
- **Private frontier AI:** Funding valuation, ARR/revenue reports, compute cost, gross margin, model quality, retention, exit path.
- **Private application AI:** Product-led growth, ROI proof, customer concentration, incumbent bundling risk, reported ARR.
- **Strategic signal only:** Important competitive input, but evidence/investability is weak; track mainly for ecosystem impact.

## P0 Public: Valuation Framework

| Company | Primary lens | Market-implied expectation to test | Mispricing criteria | Priority |
|---|---|---|---|---|
| NVIDIA | AI infrastructure compounder | AI accelerator demand and margins remain structurally high beyond the current capex cycle. | Underpriced if networking/software attach and inference sustain growth after training cycle; overpriced if hyperscaler ASICs and supply normalization compress margins. | P0-A |
| Microsoft | Platform monetization | Azure AI and Copilot can earn high returns on massive AI capex. | Underpriced if Copilot/agent ARPU and Azure AI backlog convert with margin stability; overpriced if OpenAI economics/capex dilute returns. | P0-A |
| Alphabet | Platform monetization + option value | Search cash flows survive AI disruption while Gemini/TPU/Waymo add option value. | Underpriced if search monetization remains resilient and cloud/Waymo scale; overpriced if AI answers impair ad economics faster than new revenue ramps. | P0-A |
| Amazon | AI infrastructure compounder | AWS AI, Trainium/Inferentia, ads, and logistics AI produce operating leverage despite capex. | Underpriced if AWS AI reaccelerates and retail/ads margins expand; overpriced if capex outpaces cash returns. | P0-A |
| Meta | Platform monetization | AI improves ad targeting/content engagement enough to offset capex and Reality Labs losses. | Underpriced if Llama/open AI distribution improves core ads and tools; overpriced if AI spend lacks monetization and social engagement weakens. | P0-A |
| Broadcom | Semiconductor scarcity | Custom ASIC and networking demand becomes a durable multi-year AI revenue stream. | Underpriced if hyperscaler ASIC programs broaden; overpriced if customer concentration or order pull-forward drives cycle risk. | P0-A |
| TSMC | Semiconductor scarcity | AI advanced-node and packaging demand stays supply-constrained and high-margin. | Underpriced if CoWoS/advanced packaging scarcity persists; overpriced if geopolitics or customer capex slowdown hits utilization. | P0-A |
| ASML | Semiconductor scarcity | EUV/High-NA demand remains essential for AI chip scaling. | Underpriced if High-NA adoption extends monopoly economics; overpriced if export controls/capex digestion delay orders. | P0-A |
| AMD | AI infrastructure challenger | MI accelerators become a credible second source for AI workloads. | Underpriced if software/customer wins close the gap with NVIDIA; overpriced if share gains remain narrow or margin-dilutive. | P0-B |
| Oracle | AI infrastructure + database platform | AI cloud backlog converts into profitable revenue while database estate remains sticky. | Underpriced if AI contracts convert with durable margins; overpriced if capex/leverage/customer concentration dominate. | P0-B |
| Apple | Consumer platform option value | On-device AI refreshes the device cycle and defends services economics. | Underpriced if AI drives replacement/ARPU without margin drag; overpriced if Apple remains behind cloud AI and AI is only table stakes. | P0-B |
| Tesla | Option-value battleground | Robotaxi, autonomy, robotics, and energy justify valuation far above current auto/energy earnings. | Underpriced if commercial autonomy/robotics evidence inflects; overpriced if current earnings/FCF remain the only proven value base. | P0-B |
| Palantir | Enterprise AI software | AIP becomes a durable AI operating layer for government and enterprise. | Underpriced if commercial growth and net retention compound; overpriced if valuation outruns revenue scale and contract concentration. | P0-B |
| CoreWeave | AI infrastructure pure-play | Scarce GPU cloud capacity earns durable returns despite debt/capex intensity. | Underpriced if utilization/contracts remain long-duration and pricing holds; overpriced if GPU scarcity fades or concentration/debt risk rises. | P0-C |
| Cerebras Systems | AI chip challenger | Wafer-scale systems carve out a profitable AI training/inference niche. | Underpriced if differentiated architecture wins repeat customers; overpriced if revenue concentration and operating losses persist. | P0-C |

## P1 Public First-Batch Coverage

| Company | Primary lens | Market-implied expectation to test | Mispricing criteria | Priority |
|---|---|---|---|---|
| Arm Holdings | Semiconductor IP | AI edge and datacenter designs lift royalty economics. | Underpriced if royalty rate/datacenter wins expand; overpriced if valuation embeds too much AI without near-term earnings. | P1-A |
| Qualcomm | Edge AI platform | On-device AI creates a durable handset/PC/auto upgrade cycle. | Underpriced if edge AI and auto backlog diversify revenue; overpriced if handset dependence remains dominant. | P1-A |
| Samsung Electronics | Memory/HBM cycle | HBM and memory recovery close execution gap. | Underpriced if HBM qualification improves; overpriced if lag versus SK Hynix/TSMC persists. | P1-A |
| SK Hynix | HBM scarcity | HBM pricing power and share remain durable. | Underpriced if HBM mix shift sustains margins; overpriced if capacity additions turn HBM into a commodity cycle. | P1-A |
| Micron | Memory/HBM cycle | HBM mix shift upgrades historical memory-cycle economics. | Underpriced if HBM growth changes margin profile; overpriced if DRAM cyclicality overwhelms AI mix. | P1-A |
| ServiceNow | Enterprise AI software | AI agents expand workflow wallet share. | Underpriced if AI attach lifts cRPO and retention; overpriced if model vendors/hyperscalers compress application value. | P1-B |
| Salesforce | Enterprise AI software | Agentic AI reverses seat-growth pressure and expands platform usage. | Underpriced if Agentforce drives measurable revenue uplift; overpriced if AI disrupts seat-based SaaS economics. | P1-B |
| Adobe | Creative AI software | Proprietary creative workflows and data defend against generative AI disruption. | Underpriced if Firefly/credits monetize; overpriced if AI commoditizes creative tools and churn rises. | P1-B |
| Snowflake | Data/AI platform | Enterprise data gravity remains a control point for AI apps. | Underpriced if AI workloads reaccelerate consumption; overpriced if Databricks/hyperscalers pressure growth. | P1-B |
| Datadog | AI observability | AI infrastructure complexity expands observability demand. | Underpriced if AI-native workload monitoring becomes a category tailwind; overpriced if cloud cost optimization slows usage. | P1-C |
| Uber | AI/autonomy marketplace | Mobility/logistics platform benefits from optimization and AV optionality. | Underpriced if autonomy lowers cost through partnerships; overpriced if robotaxi suppliers disintermediate marketplace value. | P1-C |
| Tencent | China AI platform | AI improves ads/games/cloud while regulation remains manageable. | Underpriced if AI monetization offsets China discount; overpriced if regulatory/geopolitical drag persists. | P1-C |
| Alibaba | China cloud/AI platform | Cloud AI and capital returns unlock undervaluation. | Underpriced if cloud AI growth and shareholder returns accelerate; overpriced if macro/regulation keeps multiple depressed. | P1-C |

## P0 Private / Unlisted: Valuation Framework

| Company | Primary lens | Valuation basis to verify | Mispricing criteria | Priority |
|---|---|---|---|---|
| OpenAI | Private frontier AI | Disclosed/reported funding valuation, reported revenue/ARR, enterprise retention, compute cost. | Underpriced if platform/API/consumer distribution compounds with improving unit economics; overpriced if compute burn, governance, and partner economics cap margins. | P0-A |
| Anthropic | Private frontier AI | Funding valuation, reported ARR, enterprise/cloud partnerships, model quality. | Underpriced if enterprise trust/safety positioning wins high-retention customers; overpriced if valuation assumes OpenAI-scale outcomes without distribution. | P0-A |
| xAI | Private frontier AI | Funding valuation, model benchmarks, X/Tesla ecosystem distribution, compute buildout. | Underpriced if unique data/distribution creates durable adoption; overpriced if governance/capital intensity and monetization lag. | P0-B |
| Databricks | Private data/AI platform | Disclosed revenue run-rate, growth, funding valuation, IPO path. | Underpriced if data platform becomes AI application control point; overpriced if public comps compress before IPO. | P0-A |
| ByteDance | Private consumer AI platform | Reported revenue/profit, secondary valuation, TikTok regulatory path, AI product traction. | Underpriced if recommendation AI/global distribution sustain growth; overpriced if geopolitics and forced-divestiture risk dominate. | P0-B |
| SpaceX / Starlink | Private AI/tech infrastructure | Funding/secondary valuation, Starlink subscribers/ARPU, launch cadence, defense contracts. | Underpriced if Starlink and defense connectivity compound as strategic infrastructure; overpriced if capex, launch risk, or liquidity premium dominate. | P0-B |
| Anduril | Private defense AI | Funding valuation, contract wins, revenue reports, product deployments. | Underpriced if defense AI procurement inflects; overpriced if long procurement cycles or margins disappoint. | P0-B |
| Perplexity | Private AI search | Funding valuation, query growth, revenue mix, partnerships, content/legal risk. | Underpriced if AI-native answer search captures high-value intent; overpriced if distribution and monetization lag incumbents. | P0-C |
| Anysphere / Cursor | Private AI coding | Reported ARR, retention, enterprise adoption, funding valuation. | Underpriced if AI coding becomes a durable workflow platform; overpriced if GitHub/Microsoft bundle away differentiation. | P0-C |
| Mistral AI | Private frontier AI | Funding valuation, revenue, government/enterprise contracts, model quality. | Underpriced if sovereign European AI demand creates durable market; overpriced if scale gap versus U.S./China labs persists. | P0-C |
| Cohere | Private enterprise AI | ARR, customer retention, cloud partnerships, funding valuation. | Underpriced if private enterprise deployments prove sticky; overpriced if hyperscaler/OpenAI/Anthropic bundling wins. | P0-C |
| Hugging Face | Private AI developer platform | Revenue, enterprise products, platform usage, funding valuation. | Underpriced if developer/model hub becomes AI infrastructure layer; overpriced if usage does not monetize. | P0-C |

## P1 Private First-Batch Monitor

| Company | Primary lens | Valuation basis to verify | Mispricing criteria | Priority |
|---|---|---|---|---|
| Groq | Private inference infrastructure | Funding valuation, throughput/cost benchmarks, customer traction, capacity. | Underpriced if low-latency inference becomes independent cloud category; overpriced if NVIDIA/custom ASICs compress niche. | P1-A |
| Figure AI | Private robotics | Funding valuation, customer pilots, unit cost, safety/autonomy milestones. | Underpriced if humanoid deployment scales with real labor ROI; overpriced if demos fail to become production economics. | P1-A |
| Physical Intelligence | Strategic robotics AI | Funding, pilots, technical benchmarks, partnerships. | Underpriced only if early evidence supports general-purpose robotics model leverage; otherwise strategic signal, not valuation-ready. | P1-C |
| Wayve | Private autonomy AI | Funding valuation, OEM partnerships, safety data, deployment path. | Underpriced if end-to-end autonomy licenses across OEMs; overpriced if validation/regulation stalls. | P1-B |
| ElevenLabs | Private AI audio | ARR/revenue, enterprise adoption, IP/regulatory risk, funding valuation. | Underpriced if voice becomes workflow/application platform; overpriced if audio models commoditize. | P1-B |
| Glean | Private enterprise AI search | ARR, net retention, enterprise logos, funding valuation. | Underpriced if enterprise knowledge search becomes control point; overpriced if Microsoft/Google bundle. | P1-B |
| Sierra | Private AI agents | ARR, customer logos, deflection/ROI metrics, retention, funding valuation. | Underpriced if customer-service agents replace large cost pools; overpriced if retention/margins are weak. | P1-B |
| Notion | Private productivity AI | ARR, user growth, enterprise adoption, AI attach, funding valuation. | Underpriced if AI workspace consolidation occurs; overpriced if AI remains a feature layer. | P1-C |
| DeepSeek | China private frontier AI | Ownership/funding clarity, model quality, adoption, cost claims. | Strategic signal for model-cost deflation and China competition; valuation work requires high evidence caution. | P1-C |
| Moonshot AI | China private AI apps | Funding valuation, user growth, revenue, product retention. | Underpriced if China AI app distribution scales; overpriced if evidence and monetization are weak. | P1-C |
| Zhipu AI | China private enterprise AI | Funding, government/enterprise contracts, model quality, policy support. | Underpriced if policy-backed enterprise adoption compounds; evidence quality and investability constraints remain high. | P1-C |

## Priority Sequencing

### First 10 deep-dive candidates

1. NVIDIA
2. Microsoft
3. Alphabet
4. OpenAI
5. Anthropic
6. Amazon
7. Meta
8. Broadcom
9. TSMC
10. Databricks

Rationale: these names define the highest-value AI infrastructure, platform, and frontier-model debates.

### Next 10

1. ASML
2. AMD
3. Oracle
4. Apple
5. Tesla
6. Palantir
7. CoreWeave
8. Cerebras Systems
9. ByteDance
10. SpaceX / Starlink

Rationale: this batch covers bottleneck suppliers, public option-value battlegrounds, and private strategic platforms.

### Private and application AI follow-up

1. xAI
2. Anduril
3. Perplexity
4. Anysphere / Cursor
5. Mistral AI
6. Cohere
7. Hugging Face
8. Groq
9. Figure AI
10. Wayve

Rationale: these require stronger source-quality work before full valuation conviction.

## Standard Mispricing Output

For each target, the final research note should end with this concise decision block:

- **Mispricing direction:** underpriced / overpriced / balanced / not enough evidence.
- **Primary driver:** current fundamentals / AI option value / market structure / cycle / strategic scarcity.
- **Evidence quality:** high / medium / low.
- **Key evidence gap:** one or two facts that would most change the conclusion.
- **Catalyst window:** near-term quarter / 6-12 months / multi-year / event-driven.
- **Confidence:** low / medium / high.

## Next Work

1. @EvidenceAnalyst should source-check the canonical list and label public/private evidence quality.
2. @ResearchManager should merge this valuation framework with the evidence-confirmation pass into the final watchlist operating document.
3. For the next individual company deep dive, start with one of the first 10 deep-dive candidates unless humans specify otherwise.
