# OpenAI L1 Pass-Through Matrix

Date: 2026-06-28
Owner: @EvidenceAnalyst
Task: #all task #33
Related tasks: #27 OpenAI valuation support, #28 OpenAI source map / data dictionary

## 1. Executive Takeaway

OpenAI is not directly investable, so the tradable question is where OpenAI's growth, compute commitments, and platform risk pass through to public L1 names.

The cleanest positive pass-through evidence is:

1. **MSFT**: equity stake, IP rights, Azure API exclusivity, revenue-share economics, and an incremental $250B Azure purchase commitment.
2. **AMZN**: $50B strategic investment plus expanded AWS / Trainium agreement, OpenAI Frontier distribution, and 2GW Trainium consumption.
3. **NVDA**: at least 10GW NVIDIA systems plus possible progressive NVIDIA investment; still core to OpenAI training and much of inference.
4. **ORCL**: Stargate / Oracle capacity is one of the largest direct OpenAI infrastructure ramps.
5. **AVGO**: confirmed 10GW custom accelerator / Ethernet collaboration and Jalapeño inference chip.
6. **CBRS**: direct OpenAI 750MW / >$20B Cerebras inference agreement, but high customer concentration and execution risk.

Second-order or more conditional pass-through:

- **TSM**: likely beneficiary of advanced-node / advanced-packaging demand behind NVIDIA and custom accelerators, but the OpenAI-to-TSM link is inferred unless chip manufacturing allocation is disclosed.
- **CRWV**: OpenAI has named CoreWeave as part of its infrastructure ecosystem and Stargate planning, but current CoreWeave disclosures need an OpenAI-specific contract/RPO bridge before valuation.
- **GOOGL**: OpenAI has named Google Cloud as one cloud provider, but the more important read-through is competitive pressure versus Gemini / Google Cloud rather than clearly confirmed OpenAI revenue capture.

The key investment discipline: **do not count the same OpenAI dollar twice.** A dollar of OpenAI revenue, a dollar of OpenAI cloud spend, a dollar of supplier revenue, and a dollar of strategic investment are different economics.

## 2. Source Quality Legend

| Label | Meaning | Valuation use |
|---|---|---|
| Confirmed direct | Official company/partner source names the OpenAI relationship and economic/capacity metric. | Can support pass-through thesis, but still needs margin/timing. |
| Confirmed relationship | Official source names the relationship but not enough economics. | Use for exposure map, not valuation weight. |
| Reported | Reputable media or third-party report, not official. | Scenario or cross-check only. |
| Inferred | Logical supply-chain link from confirmed upstream demand. | Track, but do not underwrite without disclosure. |
| Missing | Needed metric is unavailable. | Cannot support valuation conclusion. |

## 3. Core L1 Matrix

| L1 name | Pass-through route | Evidence quality | OpenAI-linked evidence | What must be true for stock upside | Main risk / double-counting trap | Next data needed |
|---|---|---|---|---|---|---|
| MSFT | Equity stake, Azure API exclusivity, OpenAI IP rights, Azure consumption, Copilot distribution | Confirmed direct | Microsoft says it holds an OpenAI Group PBC investment valued around $135B / ~27% diluted; OpenAI remains Microsoft's frontier model partner; Microsoft retains Azure API exclusivity until AGI; OpenAI contracted to purchase incremental $250B Azure services. | OpenAI usage drives Azure consumption and Copilot differentiation while Microsoft keeps attractive economics. | Microsoft lost right of first refusal as compute provider; OpenAI can use multiple clouds; capex and revenue-share economics may dilute margins. | Updated post-2026 ownership after later rounds; Azure gross margin on OpenAI workloads; Copilot revenue tied to OpenAI vs in-house models. |
| AMZN | Strategic investment, AWS distribution, Trainium capacity, Bedrock / Frontier | Confirmed direct | OpenAI / Amazon announced Amazon will invest $50B; AWS will be exclusive third-party cloud distribution provider for OpenAI Frontier; OpenAI will consume ~2GW Trainium; the $38B agreement expands by $100B over 8 years. | Trainium becomes credible frontier/inference infrastructure and OpenAI drives AWS AI workload share gain. | Investment return, compute revenue, and AWS margin are separate; Trainium adoption may require pricing concessions. | Recognition schedule for AWS revenue; Trainium utilization; margin on OpenAI capacity; whether Frontier drives incremental AWS customers. |
| NVDA | GPU systems, networking, preferred compute partner, strategic investment | Confirmed direct | OpenAI / NVIDIA announced at least 10GW NVIDIA systems; first 1GW targeted for H2 2026 on Vera Rubin; NVIDIA intends to invest up to $100B progressively as each GW deploys. OpenAI says NVIDIA remains the foundation of training and majority inference. | OpenAI remains GPU-heavy despite custom silicon and multi-cloud diversification. | Circularity risk: NVIDIA investment may support OpenAI purchases; custom silicon and Trainium can cap long-run share. | Conversion from LOI to firm purchase; revenue timing by GW; margin on Vera Rubin systems; mix shift from training to inference. |
| AVGO | Custom accelerators, Ethernet networking, Jalapeño inference chip | Confirmed direct | OpenAI / Broadcom announced 10GW custom AI accelerator collaboration; deployments targeted to start H2 2026 and complete by end-2029; Jalapeño is OpenAI's first Intelligence Processor with Broadcom silicon/networking. | OpenAI custom silicon ramps from prototype to production and Broadcom captures silicon plus networking content. | Custom chip economics may be lower-margin, lumpy, and concentrated; performance claims need production validation. | Revenue per GW / rack; Broadcom content per accelerator/network; manufacturing partner; production yield and deployment cadence. |
| TSM | Foundry / advanced packaging behind NVIDIA and custom accelerators | Inferred | OpenAI has confirmed NVIDIA, Broadcom/custom accelerator, and multi-generation chip roadmap demand; TSM is not directly named in OpenAI sources for the OpenAI chip supply chain. | OpenAI-driven GPU/custom accelerator demand increases advanced node and CoWoS-like packaging demand. | This is second-order pass-through; do not count it as a direct OpenAI contract without fabrication/packaging disclosure. | Which foundry and package are used for Jalapeño / future OpenAI accelerators; NVIDIA Vera Rubin wafer/package allocation; TSM capacity pricing. |
| ORCL | Stargate cloud/data center capacity, Oracle Cloud infrastructure, data center buildout | Confirmed direct | OpenAI announced Stargate with Oracle as an initial technology partner; later OpenAI / Oracle 4.5GW additional Stargate capacity; five-site expansion says Oracle partnership exceeds $300B over five years and takes Stargate toward the 10GW / $500B plan. | Oracle can deliver large AI capacity on time while earning acceptable cloud/data-center margins. | Large headline capacity can still be capex-heavy and financing-sensitive; "capacity" is not revenue or FCF. | Contract terms, revenue recognition, capex funding, power availability, gross margin, customer concentration, debt impact. |
| CRWV | AI cloud capacity / CoreWeave infrastructure in OpenAI ecosystem | Confirmed direct but needs bridge | OpenAI names CoreWeave among cloud/infrastructure partners and says Hopper/Blackwell systems are already in operation across Microsoft, OCI, and CoreWeave. CoreWeave reported $99.4B revenue backlog / $98.8B RPO, $2.078B Q1 2026 revenue, $1.157B adjusted EBITDA, and $740M net loss. Its risk factor names an OpenAI contract up to about $11.9B through Oct. 2030. | OpenAI/frontier lab workloads convert into durable high-utilization revenue faster than capex/debt burden rises. | Do not attribute CoreWeave's whole backlog to OpenAI. Backlog is not FCF; Q1 net interest expense, PP&E purchases, depreciation, debt and customer concentration are first-order equity claims. | OpenAI-specific RPO waterfall, contract timing, customer concentration, capex by project, debt/interest schedule, utilization. |
| CBRS | OpenAI inference capacity, Cerebras fast inference, AWS distribution | Confirmed direct | Cerebras Q1 2026 release says it announced a multi-year OpenAI deal valued at >$20B for 750MW high-speed inference compute. Task #31 notes Q1 OpenAI revenue was only $16.9M net of warrant amortization, RPO was $25.0B, and an OpenAI warrant can cover up to 33.445M Class N shares. | OpenAI validates Cerebras architecture and revenue scales beyond initial concentrated customers. | Customer concentration is explicit; >$20B contract value is not near-term recognized revenue; dilution/warrant accounting and data center/capital execution matter. | Pro forma cap table, contract terms, annual revenue conversion, OpenAI financing/loan terms, AWS distribution economics, warrant/contra-revenue treatment. |
| GOOGL | Competitive AI platform, Google Cloud optionality, Gemini benchmark pressure | Confirmed relationship / competitive read-through | OpenAI says its cloud strategy spans Microsoft, Oracle, AWS, CoreWeave, and Google Cloud. No large OpenAI/Google economic term is disclosed in current source set. | Google Cloud wins selective OpenAI workloads or Gemini/TPU stack gains credibility as alternative AI infrastructure. | OpenAI success may pressure Google Search/Gemini economics as much as it helps Google Cloud. | OpenAI-Google Cloud contract terms if any; Google Cloud AI revenue disclosure; Gemini adoption vs ChatGPT; TPU external customer economics. |

## 4. Directional Ranking

### Best confirmed positive pass-through

| Rank | Name | Why |
|---:|---|---|
| 1 | AMZN | Largest explicitly expanded AWS/Trainium agreement plus $50B strategic investment and OpenAI Frontier distribution. |
| 2 | NVDA | 10GW NVIDIA systems and up to $100B progressive investment; OpenAI still states NVIDIA is foundational. |
| 3 | MSFT | Strongest contractual/IP relationship and $250B Azure commitment, but less exclusive after OpenAI's multi-cloud shift. |
| 4 | ORCL | Large Stargate capacity build with OpenAI, but capex/financing/margin quality must be tested. |
| 5 | AVGO | Clear custom silicon/networking route, but production economics are not yet visible. |
| 6 | CBRS | Very direct OpenAI contract, but smaller company with high execution and concentration risk. |

### Most likely expectation-risk names

| Name | Why expectation risk is high |
|---|---|
| CRWV | Headline $99.4B backlog can be over-read; OpenAI-specific exposure is meaningful but smaller than total backlog and must clear capex/debt/interest hurdles. |
| CBRS | OpenAI contract validates product but can also create customer concentration, warrant dilution, contra-revenue, and financing dependence. |
| ORCL | Very large AI capacity commitments may drive revenue but also capex, debt, power, and margin uncertainty. |
| NVDA | OpenAI demand supports the bull case, but custom silicon / Trainium / Cerebras are explicit alternatives. |
| GOOGL | OpenAI success is competitively ambiguous: possible cloud customer, but also direct pressure on Gemini/Search. |

## 5. Avoiding Double Counting

| Do not mix | Correct treatment |
|---|---|
| OpenAI $852B post-money valuation | Private funding valuation anchor only; not market cap and not supplier revenue. |
| OpenAI $24B annualized official run-rate | OpenAI revenue scale; not equal to cloud spend or hardware spend. |
| Amazon / NVIDIA investment dollars | Strategic capital into OpenAI; not automatically revenue to AWS/NVIDIA. |
| Compute capacity in GW | Capacity / infrastructure scale; not revenue without price, timing, utilization, and margin. |
| RPO / backlog | Potential future revenue; needs conversion schedule, cancellations/conditions, capex and FCF bridge. |
| Supplier revenue | Supplier gross profit / FCF depends on margin and funding burden, not just demand. |

## 6. Research Checklist Before Valuation

For every L1 name, collect:

1. **OpenAI exposure type**: equity, cloud revenue, hardware sale, custom silicon, data center capacity, distribution, competitive risk.
2. **Contract status**: definitive agreement, LOI, term sheet, partnership announcement, reported only.
3. **Economics**: committed dollars, capacity, timing, revenue recognition, gross margin, capex, financing, cancellation terms.
4. **Concentration**: OpenAI as % of revenue/backlog/customer receivables if disclosed.
5. **FCF bridge**: revenue -> gross profit -> opex/capex/debt service -> FCF.
6. **Market-implied expectations**: current EV/revenue, EV/EBITDA, P/FCF, and consensus growth for listed names.

## 7. Source Index

- OpenAI, "Scaling AI for everyone": https://openai.com/index/scaling-ai-for-everyone/
- OpenAI, "OpenAI raises $122 billion to accelerate the next phase of AI": https://openai.com/index/accelerating-the-next-phase-ai/
- OpenAI, "The next phase of enterprise AI": https://openai.com/index/next-phase-of-enterprise-ai/
- OpenAI / Amazon partnership: https://openai.com/index/amazon-partnership/
- OpenAI / NVIDIA systems partnership: https://openai.com/index/openai-nvidia-systems-partnership/
- OpenAI / Broadcom strategic collaboration: https://openai.com/index/openai-and-broadcom-announce-strategic-collaboration/
- OpenAI / Broadcom Jalapeño inference chip: https://openai.com/index/openai-broadcom-jalapeno-inference-chip/
- Microsoft / OpenAI partnership update: https://blogs.microsoft.com/blog/2025/10/28/the-next-chapter-of-the-microsoft-openai-partnership/
- OpenAI, "Announcing The Stargate Project": https://openai.com/index/announcing-the-stargate-project/
- OpenAI, "Stargate advances with 4.5 GW partnership with Oracle": https://openai.com/index/stargate-advances-with-partnership-with-oracle/
- OpenAI, "OpenAI, Oracle, and SoftBank expand Stargate with five new AI data center sites": https://openai.com/index/five-new-stargate-sites/
- CoreWeave Q1 2026 results: https://investors.coreweave.com/news/news-details/2026/CoreWeave-Reports-Strong-First-Quarter-2026-Results/
- CoreWeave Q1 2026 10-Q: https://www.sec.gov/Archives/edgar/data/1769628/000176962826000222/crwv-20260331.htm
- Cerebras Q1 2026 results: https://investors.cerebras.ai/news-releases/news-release-details/cerebras-systems-announces-strong-first-quarter-2026-results
- Cerebras Q1 2026 10-Q: https://www.sec.gov/Archives/edgar/data/2021728/000162828026044981/cbrs-20260331.htm

## 8. Bottom Line

For OpenAI pass-through, the cleanest tradable structure is not "buy every AI supplier." The right structure is:

- **Confirmed strategic/cloud/hardware exposure**: MSFT, AMZN, NVDA, ORCL, AVGO, CBRS.
- **Second-order supply chain exposure**: TSM.
- **Backlog conversion / FCF risk exposure**: CRWV, ORCL, CBRS.
- **Competitive platform read-through**: GOOGL, MSFT, AMZN.

The next valuation step should assign probabilities and margin assumptions only after each company's contract timing, revenue recognition, capex burden, and customer concentration are refreshed.
