# First Attack Manager Packet

Date: 2026-06-28
Owner: ResearchManager
Scope: CBRS, CRWV, PLTR, Databricks, OpenAI

## Executive View

The first attack packet is complete enough for manager synthesis, but not yet trade-memo-ready.

The best near-term research edge is not "AI demand exists." The edge is identifying where the market is incorrectly converting AI demand into equity value.

Priority ranking:

1. CRWV / CoreWeave: highest immediate modelability. The market may misprice backlog quality and leverage, but this requires an EV-based RPO-to-FCF model.
2. CBRS / Cerebras: highest information-edge candidate. Newly public, low coverage, direct OpenAI exposure, but not per-share valuation-ready because dilution and contract conversion are unresolved.
3. PLTR: strongest hard-data software case. AIP is not just a generic story, but valuation is already tight.
4. Databricks: important IPO/event intelligence. Useful for SNOW and data-platform repricing, but needs S-1 before valuation confidence.
5. OpenAI: central private valuation anchor and demand source. Direct IPO valuation remains scenario-based; near-term PnL comes through L1 pass-through names.

## Ranking Table

| Direction | Edge | Immediacy | Data quality | Tradeability | Manager status |
|---|---|---:|---:|---:|---|
| CRWV | Backlog quality vs leverage underwriting | High | High | High | Synthesis-ready; needs EV/RPO-to-FCF valuation model |
| CBRS | New IPO, low coverage, direct OpenAI inference exposure | High | Medium | Medium-low | Synthesis-ready; not per-share valuation-ready |
| PLTR | AIP production/revenue quality vs premium multiple | Medium-high | High | High | Synthesis-ready; needs market/consensus/dilution refresh |
| Databricks | S-1 / IPO valuation anchor for SNOW and data platforms | Medium | Medium-high | Event only | Synthesis-ready; needs S-1 |
| OpenAI | Central private AI valuation and L1 pass-through anchor | High strategic value | Medium | Indirect only | Synthesis-ready; direct IPO remains scenario |

## 1. CRWV / CoreWeave

### Manager Thesis

CRWV is the most modelable near-term attack target because it has hard data: revenue, adjusted EBITDA, GAAP loss, RPO/backlog, debt, interest and PP&E purchases. The key question is whether $99.4B revenue backlog / $98.8B RPO turns into equity cash earnings after capex, depreciation, debt and interest.

### What We Know

- Q1 revenue: $2.078B.
- Adjusted EBITDA: $1.157B / 56% margin.
- GAAP net loss: $740M.
- Revenue backlog: $99.4B; SEC RPO: $98.8B.
- RPO timing: 36% in 0-24 months, 39% in months 25-48, 25% in months 49-84.
- Total debt principal: $25.149B.
- Q1 net interest expense: $536M.
- Q1 PP&E purchases: $7.695B.

### PnL Path

Bull case: the market over-discounts leverage and underprices contracted AI compute demand if near-term RPO converts on schedule and adjusted EBITDA remains high.

Bear case: the market over-capitalizes backlog while debt, interest, depreciation and growth capex absorb most economics before equity.

### Next Model

Build:

```text
RPO buckets -> revenue conversion -> adjusted EBITDA -> cash interest -> capex/PP&E -> depreciation/useful life -> equity FCF -> EV-to-equity
```

CRWV cannot be valued from market cap / sales or backlog / market cap shortcuts.

## 2. CBRS / Cerebras

### Manager Thesis

CBRS is the highest information-edge candidate because it is newly public, low coverage, pure AI-inference infrastructure and directly tied to OpenAI. But it is not per-share valuation-ready.

### What We Know

- Q1 revenue: $193.4M.
- FY26 core revenue guide: $855M-$865M.
- OpenAI 750MW commitment; company headline value >$20B.
- OpenAI Q1 recognized revenue: $16.9M net of warrant amortization.
- RPO: $25.0B.
- OpenAI warrant up to 33.445M Class N shares.
- Major unresolved items: post-IPO fully diluted share count, G42/AWS/customer warrants, SBC/RSUs/options, float/lock-up/liquidity.

### PnL Path

Bull case: market underprices a scarce public inference-infrastructure asset as OpenAI capacity tranches convert into revenue.

Bear case: headline contract/RPO gets over-capitalized before revenue, gross profit and per-share economics are visible.

### Next Model

Build:

```text
OpenAI/G42/AWS contract schedule -> revenue recognition -> gross profit -> warrant amortization/dilution -> leases/capex -> fully diluted EV/share
```

CBRS should stay on the high-upside watchlist, but no trade memo until dilution, warrants, leases and liquidity are solved.

## 3. PLTR / Palantir

### Manager Thesis

PLTR is not a fake AI story. The hard data supports premium diligence: growth, U.S. commercial expansion, RDV/RPO, customer/deal metrics, margin and FCF are all moving in the right direction. But the valuation already prices in exceptional execution.

### What We Know

- Q1 revenue growth: +85% YoY.
- U.S. commercial revenue growth: +133% YoY.
- NDR: 150%.
- U.S. commercial RDV: +112% YoY.
- Adjusted operating margin: 60%.
- FY2026 adjusted FCF guide: $4.2B-$4.4B.
- Valuation snapshot: about 37x FY2026 revenue and 67x FY2026 adjusted FCF.

### PnL Path

Bull case: AIP converts from pilot to production, sustaining exceptional commercial growth, retention and FCF quality.

Bear case: market over-capitalizes early AIP momentum; RDV does not convert; SBC/dilution and multiple compression hurt per-share value.

### Next Model

Before trade memo:

- verified adjusted close / 前复权 history,
- formal consensus,
- EV/NTM revenue and FCF comps,
- SBC/dilution bridge,
- RDV/RPO conversion tracker.

PLTR is synthesis-ready, not trade-memo-ready.

## 4. Databricks

### Manager Thesis

Databricks is a high-readiness IPO/event watch item and a valuation anchor for SNOW and the broader data/AI software stack. It is not yet a direct trade.

### What We Know

- Revenue run-rate: $5.4B.
- Growth: strong enough to support IPO readiness, but needs S-1 audit proof.
- Official valuation anchor: $134B.
- $134B equals about 24.8x disclosed run-rate revenue.
- SNOW anchor: about 14.7x based on the peer sheet snapshot.

### Valuation Framing

- $100B: supportable if S-1 quality is strong.
- $134B: defensible but demanding; requires premium evidence vs SNOW.
- $175B: stretch / platform-option case, not base case.

### PnL Path

The edge is event intelligence:

- If S-1 shows strong growth, NRR, AI product attach and FCF quality, Databricks can support a premium and lift data-platform comps.
- If S-1 quality disappoints, SNOW and high-multiple data/AI software peers can reprice lower.

### Next Model

Wait for S-1 or audited disclosures. Until then, do not treat private run-rate revenue and preferred-share valuation like public GAAP revenue and public common-equity market cap.

## 5. OpenAI

### Manager Thesis

OpenAI is the central private AI valuation anchor, but the direct IPO valuation is still scenario-based. The more actionable public-market work is L1 pass-through: which listed companies capture OpenAI-related economics without double-counting.

### What We Know

- Official run-rate anchor: $2B/month, about $24B annualized.
- Official private valuation anchor: $852B post-money.
- $1T base-case support test needs roughly $190B 2030 revenue and about $48B 2030 FCF.
- $1T bull case still needs roughly $123B 2030 revenue.
- Gross margin, burn, inference unit cost, partner economics, retention and IPO/governance remain critical gaps.

### Pass-Through View

Cleanest positive public pass-through:

- AMZN
- MSFT
- NVDA
- AVGO

Direct but risk-heavy:

- ORCL
- CBRS
- CRWV

Second-order / ambiguous:

- TSM
- GOOGL

### Main Rule

Do not double-count. Separate:

- OpenAI ownership value,
- OpenAI revenue,
- cloud revenue,
- hardware revenue,
- strategic investment dollars,
- compute capacity,
- RPO/backlog,
- competitive pressure.

OpenAI should guide public-stock research, not become a direct $1T base-case equity story yet.

## Current Action Plan

### Immediate Work

1. CRWV: build full EV-based RPO-to-equity-FCF model.
2. CBRS: build fully diluted cap table and contract-conversion bridge.
3. PLTR: refresh adjusted close / consensus / EV comps / dilution / RDV conversion.
4. OpenAI: convert pass-through matrix into L1 name-by-name valuation sensitivities.
5. Databricks: wait for S-1, but keep valuation scenario and SNOW peer monitor active.

### What Not To Do

- Do not write buy/sell trade memos from current headline metrics.
- Do not capitalize OpenAI deal value, CRWV backlog, CBRS RPO or Databricks private valuation as if they were public equity value.
- Do not mix private preferred valuation with public common-equity market cap.
- Do not use unrefreshed market data for final trade conclusions.

## CEO-Level Summary

We now have five attack directions, but the first real PnL question is narrower:

> The market sees AI demand. We need to find where the market miscalculates how much of that demand becomes durable per-share cash value.

CRWV and CBRS are the most misread infrastructure cases. PLTR is the strongest software execution case, but valuation is tight. Databricks is an IPO repricing event for data-platform peers. OpenAI is the demand and valuation anchor, but the trade is mostly through public pass-through names until IPO economics are visible.

The next best use of time is not more broad evidence collection. It is model construction on the conversion bottlenecks:

- backlog to FCF,
- contract value to per-share value,
- AIP adoption to durable revenue,
- private valuation to public comp,
- OpenAI demand to L1 public-stock economics.
