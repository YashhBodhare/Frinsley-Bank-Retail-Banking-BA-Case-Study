# Source Notes, Assumptions, and Decision Log

## Source reviewed

**File:** `Course Project - Frinsley Bank.pptx` (four slides). The source title and module briefs use “Frinsley Bank.” The project owner confirmed the correct project spelling is Frinsley (F-R-I-N-S-L-E-Y).

## Facts explicitly present in the source

- The bank is newly launched and has a banking license.
- Banking, credit cards, home loans, and mutual funds are named as services.
- A managing committee and project team will decide the product launch plan.
- A retail banking software application is to be developed by an IT company named “Solutions Inc.” in the presentation.
- The product owner has started meetings with bank stakeholders; the BA is part of the elicitation team and is tasked with starting user stories.
- Credit-card functions listed: card details view, current statement, last statement, detailed statement, and credit-card balance payment.
- Banking functions listed: bank account details, bank statements, funds transfer using NEFT/RTGS/IMPS, login, unified view, and utility payments.
- The presentation calls for problem statement, user stories, user-story cards/prototypes, process diagram if applicable, assumptions, and constraints.

## Source inconsistencies and interpretation

1. **Project 02 heading:** The banking project slide says “the credit card module” immediately before listing bank account, statement, transfer, login, unified-view, and utility-payment features. This appears to be a copy/paste label; the pack interprets those functions as the Banking module and records the source issue here.
2. **“Current”, “last”, “detailed” statement:** These are source terms, but no definitions, periods, or data formats are supplied.
3. **Release sequence:** The deck says credit cards and banking are “next in the priority list,” while also saying the committee/project team will decide the launch plan. Treat scope/order as provisional until decision is recorded.

## Important missing information

- Jurisdiction and applicable regulatory/control requirements.
- Customer personas, eligibility, account/card ownership and access rules.
- Web/mobile channel, language, accessibility target, and supported devices.
- Payment rail rules: limits, fees, cut-offs, beneficiary validation, authentication, settlement, pending/reversal/refund, and reconciliation.
- Utility provider/biller scope and integration behavior.
- Card payment funding source, amount options, allocation, payment timing, and due-date handling.
- System architecture, source-of-truth systems, API contracts, data freshness, availability, performance, retention, audit and security controls.
- Interview notes, survey results, stakeholder names, approvals, budget, schedule, story points, and actual UAT results.

## Assumption register

| ID | Assumption used in draft | Validation owner |
|---|---|---|
| A-01 | Retail customers are the primary users | Product owner |
| A-02 | Digital app users may have multiple authorized bank products | Product/identity |
| A-03 | Statements and transaction data are available from authoritative bank services | Technology/data owners |
| A-04 | Transfer types listed in the deck can be selectively enabled for this release | Payments operations/product |
| A-05 | Customer support is needed for unresolved transaction/service issues | Operations |
| A-06 | The two named modules can be analyzed together while release order remains open | Sponsor/product owner |

## Decision log

| ID | Decision needed | Owner | Status |
|---|---|---|---|
| D-01 | Use the confirmed institution name spelling: Frinsley | Project owner | Resolved |
| D-02 | Confirm whether Project 02 is the Banking module | Product owner | Open; analyst interpretation is Banking |
| D-03 | Approve release order and scope boundary for each module | Managing committee / sponsor | Open |
| D-04 | Confirm channel(s) and supported customer/device profile | Product/technology | Open |
| D-05 | Approve transfer and card-payment rules and state model | Payments/card operations, risk, security | Open |
| D-06 | Confirm applicable security, privacy, regulatory, and audit requirements | Compliance/security/legal | Open |
| D-07 | Approve success measures and numeric targets | Sponsor/product owner | Open |

## Publication checklist

- D-01 is resolved. Confirm D-02 and the release decisions before presenting module scope and sequence as approved.
- Replace current-state hypotheses with evidence from actual process discovery.
- Label research as planned until real interviews/survey results are collected.
- Keep fictional/simulated portfolio examples separate from real customer data.
- Obtain SME review for banking controls and payment behavior; this pack is not policy advice.
