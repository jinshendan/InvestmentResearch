# Final AI/Tech Watchlist: Two-Layer Structure

Date: 2026-06-27
Owner: @ResearchManager
Update basis: @huiru-gao instruction to replace the five-batch structure with two layers:
- L1: 29 listed/public targets
- L2: 22 private/unlisted targets

Inputs:
- Prior final coverage order: `reports/final_canonical_watchlist_coverage_order_2026-06-27.md`
- Watchlist v1 canonical: `/Users/sjin/.slock/agents/9fe4b418-f779-408f-b283-2db54e8d8735/reports/ai_tech_target_watchlist_v1_canonical_2026-06-27.md`
- Valuation framework task #8: `/Users/sjin/.slock/agents/9fe4b418-f779-408f-b283-2db54e8d8735/reports/ai_tech_watchlist_valuation_framework_v1_2026-06-27.md`
- Evidence confirmation task #9: `/Users/sjin/.slock/agents/6dbffcc0-c910-4ee6-97ea-736e4a918272/reports/watchlist_evidence_confirmation_task9_2026-06-27.md`

## Core Change

The previous five-batch ordering mixed public, private, infrastructure, platform, and application names. Per @huiru-gao, the canonical operating structure is now two layers:

- **L1: listed/public investable targets** where market price, adjusted-close history, financials, valuation, and mispricing can be directly analyzed.
- **L2: private/unlisted targets** that mainly affect L1 valuation assumptions, provide IPO/event optionality, or serve as strategic intelligence.

This structure is cleaner for portfolio/research workflow because public names can be priced directly, while private names require evidence-quality and listing-probability handling.

## L1: Listed/Public Targets

Total: 29.

### L1-A: Core Compute

Purpose: Direct AI compute supply chain, bottlenecks, and scarcity economics.

| Company | Ticker | Primary mispricing question |
|---|---:|---|
| NVIDIA | NVDA | Are AI accelerator demand, margins, networking attach, and CUDA lock-in more durable than the market expects? |
| Broadcom | AVGO | Are custom ASIC and AI networking revenues structurally underpriced, or too concentrated in a few hyperscalers? |
| TSMC | TSM | Is advanced-node and CoWoS scarcity a multi-year structural moat, or does geopolitics/capex cycle dominate? |
| ASML | ASML | Is EUV/High-NA monopoly value underpriced relative to export-control and semiconductor-cycle risk? |
| AMD | AMD | Can AMD become a credible AI accelerator second source with enough software/customer traction? |
| Samsung Electronics | 005930.KS | Can Samsung close HBM/foundry gaps and benefit from AI memory demand? |
| SK Hynix | 000660.KS | Is HBM pricing power and share durability underpriced? |
| Micron | MU | Is HBM structurally upgrading the historical DRAM cycle? |
| Arm Holdings | ARM | Can edge and data-center AI lift royalty economics enough for valuation? |
| Qualcomm | QCOM | Is edge AI/data-center optionality underpriced versus handset dependence? |

### L1-B: Cloud and Platforms

Purpose: Public platforms whose valuations are directly affected by cloud AI demand, private-model partners, and capex ROI.

| Company | Ticker | Primary mispricing question |
|---|---:|---|
| Microsoft | MSFT | Can Azure AI and Copilot earn high returns on AI capex, and how should OpenAI economics be valued? |
| Amazon | AMZN | Is AWS AI growth/capex payback underpriced or is FCF pressure dominant? |
| Alphabet | GOOGL | Is the market overpricing AI search disruption and underpricing Gemini/TPU/Waymo/cloud option value? |
| Oracle | ORCL | Will AI RPO/backlog convert into profitable revenue despite customer concentration and capex burden? |
| CoreWeave | CRWV | Does scarce GPU cloud capacity justify public valuation despite debt, concentration, and backlog conversion risk? |

### L1-C: Applications and Software

Purpose: Public software/application platforms where AI monetization, AI attach, productivity, and bundling risk drive mispricing.

| Company | Ticker | Primary mispricing question |
|---|---:|---|
| Meta Platforms | META | Is AI-driven ad efficiency and Llama/open-model distribution underpriced relative to capex and Reality Labs drag? |
| Apple | AAPL | Can on-device AI refresh the installed base and services ARPU, or is AI table stakes? |
| Palantir | PLTR | Does AIP become a durable operating layer for government/enterprise AI, or is valuation ahead of scale? |
| ServiceNow | NOW | Can Now Assist and autonomous workflow automation drive enterprise wallet-share expansion? |
| Salesforce | CRM | Can Agentforce reverse seat-based SaaS pressure and create measurable AI ARR? |
| Adobe | ADBE | Does Firefly/AI-first ARR offset generative AI disruption risk to creative tools? |
| Snowflake | SNOW | Can AI workloads reaccelerate data consumption versus Databricks/hyperscaler competition? |
| Datadog | DDOG | Is AI infrastructure complexity creating a durable observability tailwind? |

### L1-D: High-Controversy Option Value

Purpose: Public names where valuation depends heavily on long-duration option value and where mispricing can be extreme.

| Company | Ticker | Primary mispricing question |
|---|---:|---|
| Tesla | TSLA | Is autonomy/robotaxi/robotics/energy option value over- or underpriced relative to current auto/energy fundamentals? |
| Cerebras Systems | CBRS | Can wafer-scale AI systems become a repeatable, profitable niche beyond concentrated deals? |
| Uber | UBER | Does AI/autonomy enhance marketplace economics or create disintermediation risk from robotaxi suppliers? |

### L1-E: China AI

Purpose: Listed China AI/platform exposure, including the Zhipu classification correction.

| Company | Ticker | Primary mispricing question |
|---|---:|---|
| Tencent | 0700.HK | Is AI ad/cloud/game monetization underpriced within China regulatory/geopolitical discount? |
| Alibaba | BABA / 9988.HK | Is cloud AI growth and capital return underpriced against China macro/regulatory drag? |
| Zhipu / Z.ai / Knowledge Atlas Technology | 2513.HK | Classification correction: evaluate as HK-listed China AI/model company, not pure private; mispricing depends on liquidity, disclosure, model traction, and geopolitical risk. |

## L2: Private / Unlisted Targets

Total: 22.

L2 names are not analyzed like public stocks. Each review must include listing probability, likely listing venue/path, valuation-source quality, direct investability, and which L1 valuation assumptions the company affects.

### L2-A: Directly Affect L1-B Valuation

These companies directly affect cloud/platform valuations, especially Microsoft, Alphabet, and Amazon.

| Company | Primary linked L1 names | Why it matters |
|---|---|---|
| OpenAI | MSFT | Drives Microsoft/OpenAI economics, Azure AI demand, enterprise AI platform expectations, and capex returns. |
| Anthropic | AMZN, GOOGL | Affects AWS/Google Cloud AI demand, model-platform competition, and private frontier AI valuation marks. |

### L2-B: Affect L1-A Compute Demand Assumptions

These names change demand assumptions for AI compute, HBM, cloud infrastructure, model training/inference, and data infrastructure.

| Company | Primary linked L1 names | Why it matters |
|---|---|---|
| xAI | NVDA, AVGO, TSM, AMD, CoreWeave | Large-scale frontier compute buildout affects accelerator/cloud demand, but revenue and related-party economics are major gaps. |
| Databricks | MSFT, AMZN, GOOGL, SNOW, NVDA | Data/AI platform demand affects cloud consumption and enterprise AI workload assumptions. Also has IPO-candidate relevance. |

### L2-C: Independent Major Event / IPO Candidates

These private names may become standalone public-market events. Databricks has dual relevance: compute-demand driver and IPO candidate.

| Company | Primary event path | Why it matters |
|---|---|---|
| SpaceX / Starlink | Starlink or SpaceX liquidity/listing path | Major deep-tech infrastructure asset with direct strategic and communications value; financial estimates need caution outside prospectus disclosures. |
| ByteDance | IPO, forced divestiture, secondary liquidity, or restructuring | Massive private platform with recommendation AI and consumer distribution; revenue/valuation remain reported, not company-disclosed. |
| Databricks | IPO candidate | Strong revenue run-rate and AI product traction; public comp/multiple compression matters before IPO. |

### L2-D: Strategic Intelligence / Optionality

These names inform the ecosystem, competitive threat, or future IPO pipeline. They should be tracked, but most require heavier source-quality caution before full valuation conclusions.

| Company | Segment | Main reason to track |
|---|---|---|
| Anduril | Defense AI/autonomy | Defense AI procurement and autonomous systems adoption. |
| Perplexity | AI search | Possible search behavior disruption; valuation/usage data mostly reported. |
| Anysphere / Cursor | AI coding | Clear AI-native productivity category with ARR and developer adoption signals. |
| Mistral AI | Frontier / sovereign AI | European sovereign AI and open-weight competitive signal. |
| Cohere | Enterprise / sovereign AI | Enterprise private deployments and regulated-sector AI demand. |
| Hugging Face | AI developer platform | Open-source model/distribution infrastructure and enterprise monetization. |
| Groq | AI inference infrastructure | Inference cost/latency pressure and independent inference-cloud viability. |
| Figure AI | Humanoid robotics | Physical AI deployment and labor-substitution option value. |
| Physical Intelligence | Robotics foundation models | Strategic robotics model signal; commercial evidence still thin. |
| Wayve | Autonomous driving AI | End-to-end autonomy software and OEM/robotaxi licensing path. |
| ElevenLabs | AI audio | Generative voice workflow platform potential and rights/legal risk. |
| Glean | Enterprise AI search | Enterprise knowledge retrieval and agent workflow control point. |
| Sierra | AI customer-service agents | Measurable AI-agent ROI in customer support. |
| Notion | Productivity AI | Workspace consolidation and AI-agent productivity adoption. |
| DeepSeek | China private model lab | Strategic signal for model-cost compression and China substitute pressure; weak direct investability. |
| Moonshot AI / Kimi | China private AI app/model | China AI app traction and possible listing/restructuring path; financial transparency weak. |

## Private AI Listing Probability Analysis Framework

For every L2 company, add this block before any valuation conclusion:

| Field | Required treatment |
|---|---|
| Current status | Private, unlisted, secondary-market traded, restructuring, or listing candidate. |
| Likely listing path | IPO, direct listing, SPAC/reverse merger, spin-off, tender/secondary-only, strategic acquisition, or no clear path. |
| Likely venue | U.S., HK, Europe, dual-track, unknown. |
| Listing probability | High / medium / low, with evidence. |
| Time horizon | 0-12 months, 12-24 months, 24+ months, unknown. |
| Evidence label | Company-disclosed / reported / secondary / rumored. |
| Investability today | Direct, private round only, secondary only, indirect via L1 public exposure, not investable. |
| Main public proxy | Which L1 name captures the economic exposure, if any. |
| Main blocker | Disclosure, governance, geopolitics, profitability, capex, regulatory, ownership, liquidity, or market window. |

## Immediate L2 Listing Probability Priorities

| Priority | Company | Reason |
|---:|---|---|
| 1 | Databricks | Strong revenue run-rate, positive FCF disclosure, IPO plausibility, and direct effect on cloud/data comps. |
| 2 | SpaceX / Starlink | Major private asset with possible Starlink listing/spin-off path and strategic impact. |
| 3 | ByteDance | Large-scale private platform with major event risk from TikTok/geopolitics. |
| 4 | OpenAI | Most important private AI valuation mark; listing path unclear but market impact is highest. |
| 5 | Anthropic | Strategic frontier AI asset tied to AMZN/GOOGL and private AI valuation marks. |
| 6 | Anysphere / Cursor | Clear AI application revenue signal and potential IPO pipeline candidate. |
| 7 | Anduril | Defense-tech procurement tailwind and possible long-term IPO candidate. |
| 8 | Moonshot AI / Kimi | Explicit reported HK listing/restructuring signals need verification. |
| 9 | xAI | Major compute-demand driver; listing path unclear due governance/ecosystem overlap. |
| 10 | Figure AI | High-profile robotics asset; listing probability lower near-term but strategically important. |

## Revised Workflow

1. Maintain the L1/L2 two-layer structure as canonical.
2. For L1, run normal public-market mispricing research using adjusted close / 前复权 price basis.
3. For L2, first run listing probability and evidence-quality analysis, then analyze impact on L1 valuation assumptions.
4. Do not mix L1 and L2 into one ranked public-equity queue.
5. Use L1-A/L1-B as the default first public deep-dive source unless humans specify otherwise.
6. Run a separate L2 listing-probability project before using private marks in valuation conclusions.

## Recommended Next Tasks

1. **Public deep dive:** NVIDIA as the first L1-A target, unless humans specify another public target.
2. **Private AI listing analysis:** Databricks, SpaceX/Starlink, ByteDance, OpenAI, Anthropic, Anysphere/Cursor, Anduril, Moonshot AI/Kimi, xAI, Figure AI.
3. **Watchlist document update:** Replace the prior five-batch final document with this L1/L2 taxonomy in future references.
