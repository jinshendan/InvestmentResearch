# CBRS Follow-Up: Pro Forma Cap Table + Contract-Quality Bridge

Date: 2026-06-28
Owner: @SemisAIInfraEvidenceScout
Task: #31

## Purpose

Do not value CBRS from headline Q1 revenue, the >$20B OpenAI announcement, or $25.0B RPO alone. This bridge defines the cap table, dilution, customer warrants, contract economics, lease/capex obligations, and liquidity fields that must be solved before a valuation model is reliable.

Primary sources:
- Q1 FY2026 results: https://investors.cerebras.ai/news-releases/news-release-details/cerebras-systems-announces-strong-first-quarter-2026-results
- Q1 2026 10-Q: https://www.sec.gov/Archives/edgar/data/2021728/000162828026044981/cbrs-20260331.htm

## Confirmed Starting Point

| Area | Confirmed item | Why it matters |
| --- | --- | --- |
| Public status | Nasdaq listing began May 14, 2026; IPO closed May 15, 2026. Q1 statements do not include IPO impact. | Must use post-IPO share count and cash, not just March 31 balance sheet. |
| Q1 revenue | GAAP revenue $193.4M; hardware $110.6M; cloud/other services $82.8M. | Current revenue base is small relative to contract/RPO narrative. |
| FY26 guide | Core revenue guide $855M-$865M; core gross margin 38%-41%; core operating margin negative 28%-32%. | First valuation anchor should use guided core revenue and losses. |
| OpenAI contract | OpenAI committed to 750MW inference capacity, deployed in tranches 2026-2028, with option for another 1.25GW by 2030; company says deal value >$20B. | Contract value must be converted into revenue timing, margin, and capital requirements. |
| OpenAI Q1 revenue | $16.9M net of $0.8M warrant amortization. | Early recognized revenue is tiny vs headline contract size. |
| RPO | $25.0B remaining performance obligations at March 31, 2026, with significant amount attributable to OpenAI MRA. | Bull thesis depends on RPO quality and conversion. |
| Customer concentration | Two 10%+ revenue customers were 63% and 11% of Q1 revenue and are related parties; three customers were 86% of AR. | Revenue quality and credit exposure are concentrated. |
| Customer warrants | OpenAI warrant up to 33.445M Class N shares at near-zero exercise price; G42 warrant exercised in Q2; warrant assets reduce revenue over time. | Fully diluted market cap and revenue recognition both require warrant adjustment. |
| Liquidity/capital | Q1 cash/restricted cash/short-term investments $3.3B; IPO gross proceeds $6.4B; April revolver up to $850M. | Cash runway and data-center funding capacity are post-IPO variables. |
| Data-center obligations | Q1 non-commenced lease commitments about $2.3B; Q2 additional lease commitments about $1.6B. | Contract conversion requires capacity buildout and lease/capex funding. |

## Pro Forma Cap Table Checklist

| Field | Current status | Required model treatment |
| --- | --- | --- |
| Basic shares outstanding post-IPO | Data gap in current summary. | Pull latest 10-Q/424B/8-K share table; use post-IPO count. |
| Class N / other share classes | OpenAI warrant references Class N shares. | Map all economic share classes to common-equivalent shares. |
| OpenAI warrant | Up to 33.445M Class N shares at near-zero exercise price. | Treat as in-the-money dilution unless contractual vesting/performance limits say otherwise. |
| G42 warrant | Exercised in Q2. | Include actual shares issued and any remaining related-party economics. |
| AWS warrant / strategic equity | Mentioned as partnership risk/optionality, economics need confirmation. | Do not include in diluted share count until source terms are found; flag as pending. |
| SBC / RSUs / options | Not solved in v1. | Add treasury-stock / if-converted dilution from latest filing. |
| IPO shares and greenshoe | Not solved in v1. | Add primary shares issued and cash proceeds; verify underwriter option. |
| Lock-up and float | Data gap. | Separate total diluted market cap from tradable float; important for low-coverage edge. |

### Cap Table Formula

```
fully_diluted_shares =
  post_ipo_basic_shares
  + in_the_money_options_rsus
  + OpenAI_warrant_shares
  + G42_exercised_warrant_shares
  + any_other_customer_or_partner_warrants

fully_diluted_market_cap =
  fully_diluted_shares * current_share_price

enterprise_value =
  fully_diluted_market_cap
  + debt
  + lease/debt-like obligations if valuation policy includes them
  - pro_forma_cash_and_short_term_investments
```

## Contract-Quality Bridge

| Customer / source | Confirmed economics | Revenue conversion questions | Risk label |
| --- | --- | --- | --- |
| OpenAI | 750MW committed capacity; deployment tranches 2026-2028; option for 1.25GW by 2030; deal value >$20B; Q1 recognized revenue $16.9M net of $0.8M warrant amortization. | What is annual minimum revenue by tranche? What capacity acceptance tests trigger billing? Can OpenAI delay/cancel? What gross margin after data-center/power costs? How much warrant amortization reduces revenue each period? | Highest importance; confirmed contract but conversion/margin/dilution unresolved. |
| G42 | Related party; warrant exercised in Q2; one of key historical counterparties. | How much ongoing revenue/backlog remains post-IPO? Is G42 still a demand source or mainly historical? What share issuance/dilution resulted from warrant exercise? | Related-party concentration / dilution risk. |
| AWS | Partnership referenced in v1 review; exact economics not solved. | Is there a revenue commitment, marketplace resale, co-selling, cloud-capacity obligation, or only strategic distribution? Any warrants/equity or preferred economics? | Do not model as committed revenue until terms are sourced. |
| Other customers | Two 10%+ customers are 63% and 11% of Q1 revenue; three customers are 86% of AR. | How quickly can non-OpenAI/G42/AWS customers diversify revenue? What customer-level gross margin and credit terms? | Concentration risk remains high. |

## Revenue / RPO Conversion Model

| Input | Current figure | Model action |
| --- | --- | --- |
| FY26 core revenue guide | $855M-$865M | Use as base-year revenue anchor; do not annualize Q1 alone. |
| RPO | $25.0B | Split into OpenAI vs non-OpenAI if disclosed later; otherwise scenario-test conversion. |
| OpenAI Q1 recognized revenue | $16.9M net | Build quarterly ramp scenarios: slow / base / accelerated. |
| Contract headline | >$20B OpenAI deal value | Treat as undiscounted potential contract value, not revenue or cash. |
| Gross margin guide | 38%-41% FY26 core gross margin | Use as sanity check for service/cloud ramp. |
| Operating margin guide | negative 28%-32% FY26 core operating margin | Avoid DCF profitability assumptions before opex scale proof. |

### OpenAI Conversion Scenarios

| Scenario | What must happen | Red flag |
| --- | --- | --- |
| Bull | Capacity tranches accepted on time; revenue ramps from $16.9M Q1 to material quarterly run-rate in 2H26; warrant amortization manageable; margins stay near guide. | Q2/Q3 OpenAI revenue does not step up. |
| Base | Revenue ramps but remains capex/lease constrained; FY26 guide met; RPO conversion more visible in 2027-2028. | Market prices 2028 value without 2026 execution proof. |
| Bear | Contract headline remains far ahead of realized revenue; capacity, power, or customer timing delays; dilution/warrant accounting suppresses economics. | RPO grows but revenue/margin/cash do not. |

## Lease / Capex / Liquidity Bridge

| Item | Confirmed figure | Interpretation |
| --- | --- | --- |
| Cash/restricted cash/ST investments | $3.3B at March 31, 2026, before IPO close. | Liquidity base strong but pre-IPO. |
| IPO gross proceeds | $6.4B. | Add to pro forma cash, net of fees/use of proceeds. |
| Revolver | Up to $850M April revolver. | Backup liquidity, not free equity value. |
| Non-commenced leases | $2.3B Q1 commitments and $1.6B Q2 additional commitments. | Capacity conversion requires large committed lease obligations. |

## Decision Gate Before Valuation

CBRS can move into a valuation model only after these are solved:

1. Fully diluted post-IPO share count including OpenAI/G42/customer warrants.
2. Pro forma cash/debt/lease obligations after IPO and Q2 commitments.
3. OpenAI annual revenue schedule by tranche or scenario waterfall.
4. Warrant amortization impact on revenue by customer.
5. Tradability: float, lock-up, ADV, options liquidity, borrow availability.

## Initial Model Recommendation

Use a three-scenario model:

- Revenue: FY26 guide base, OpenAI ramp sensitivity, non-OpenAI customer diversification.
- Margin: core gross margin 38%-41% as near-term anchor, then scenario-based cloud/services scale.
- Dilution: run valuation on fully diluted market cap, not headline market cap.

Until those fields are filled, the correct conclusion is "high-potential edge, not yet valuation-ready."

