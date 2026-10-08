# Project Baseline

## 1. Problem statement

**Source fact:** Frinsley Bank is described as a newly licensed bank preparing to offer banking, credit cards, home loans, and mutual funds. The managing committee and project team will decide the launch sequence. A technology partner is expected to develop the retail-banking application. The product owner has begun stakeholder meetings, and the elicitation team has been asked to start user stories.

**Analyst draft:** Customers and bank staff need a secure digital channel to view banking and card information and perform selected servicing tasks. The initial candidate scope comprises credit-card servicing and core banking self-service. The project should define a release-ready, testable scope before implementation begins.

## 2. Objectives proposed for validation

- Let an authenticated customer view eligible bank accounts and credit cards in one place.
- Let the customer inspect account/card details and statements.
- Let the customer initiate a supported bank transfer or utility payment.
- Let the customer view card statements and initiate a card balance payment.
- Give the customer clear transaction status and next steps.
- Give product, operations, technology, risk, security, and compliance stakeholders a shared, traceable requirements baseline.

These objectives are analyst proposals; the source deck does not include measurable targets or approved business outcomes.

## 3. Scope baseline

| Scope area | Included in this case-study baseline | Status |
|---|---|---|
| Credit-card servicing | Card details; current statement; last statement; detailed statement; balance payment | Source features; behavior to validate |
| Banking self-service | Login; unified view; bank-account details; bank statements; funds transfer using NEFT, RTGS, IMPS; utility payments | Source features; behavior to validate |
| Home loans and mutual funds | Mentioned as bank services | Candidate future scope; no detailed requirements supplied |
| Product launch plan | Managing committee/project team to decide | Out of scope for this BA draft; release dependency |
| Build and deployment | Application development by technology partner is described | Delivery method, channels, integrations and NFRs unconfirmed |

## 4. Primary actors (draft)

Retail customer; product owner; branch/contact-centre operations; payments operations; card operations; technology delivery team; information security; risk/compliance; utility/payment partners. These are candidate roles to validate, not a confirmed stakeholder roster.

## 5. Success measures to define

Agree baselines and targets for successful task completion, transaction failure/reversal, statement retrieval time, customer support contacts, onboarding/login completion, accessibility, and service availability. No numeric targets are available in the supplied brief.

## 6. Dependencies and constraints to confirm

- Managing committee product/release sequencing decision.
- Product and account eligibility rules.
- Payment rails, partner connectivity, operating windows, limits, charges, cut-offs, reversals, and status semantics.
- Authentication, step-up verification, session controls, device support, and fraud controls.
- Data classification, privacy, retention, audit, accessibility, and applicable compliance requirements.
- Core banking, card processing, identity, payment, and utility-provider integrations.
- Web/mobile channel scope, supported locales/currencies, and customer support model.
