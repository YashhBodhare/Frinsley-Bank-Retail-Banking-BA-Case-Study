# Business Requirements Document (BRD)

**Status:** Analyst draft for stakeholder review  
**Business area:** Digital retail banking  
**Project name:** Frinsley Bank (spelled F-R-I-N-S-L-E-Y), confirmed by the project owner and matching the source presentation.

## 1. Executive summary

The bank is preparing phased launch of banking, credit-card, home-loan, and mutual-fund services. The supplied brief identifies credit-card servicing and banking as candidate modules for a retail-banking application. This BRD frames the business need, scope, stakeholders, high-level requirements, assumptions, risks, and measures for review. It does not establish approved bank policy.

## 2. Business need

A new bank needs a coherent customer channel for selected account and card servicing. A shared application could make product information and routine servicing available digitally, provided that transaction controls, data integrity, customer eligibility, operational support, and integrations are designed and approved.

## 3. Business objectives (proposed)

- Provide a reliable digital route to account and card information.
- Enable customers to review statements and initiate in-scope payment tasks.
- Reduce avoidable manual servicing while preserving clear support and exception handling.
- Establish a traceable, testable scope aligned with the bank’s phased product rollout.

## 4. Business requirements

| ID | Requirement | Priority | Source/status |
|---|---|---|---|
| BR-01 | The solution shall support the bank’s approved launch sequence and release boundaries. | Must | Source context; sequencing decision pending |
| BR-02 | An eligible customer shall be able to access banking and card servicing through the approved digital channel. | Must | Analyst draft |
| BR-03 | Customers shall be able to view relevant account and card details and statements. | Must | Derived from source features |
| BR-04 | Customers shall be able to initiate supported bank transfers using selected NEFT, RTGS, and IMPS options. | Must | Source feature; rules and availability to validate |
| BR-05 | Customers shall be able to initiate supported utility payments. | Should | Source feature; biller scope to validate |
| BR-06 | Customers shall be able to initiate a credit-card balance payment. | Must | Source feature; funding/allocation rules to validate |
| BR-07 | The solution shall show understandable outcomes for completed, pending, and unsuccessful requests. | Must | Analyst draft; status contract to validate |
| BR-08 | Sensitive access and transactions shall comply with bank-approved security, risk, privacy, audit, and compliance requirements. | Must | Control requirement; policies to be supplied |
| BR-09 | The business shall define target measures and compare them against an agreed baseline. | Should | Analyst draft; metrics not supplied |

## 5. Scope

### In scope for this case-study baseline

Credit-card details and statements; credit-card balance payment; banking login; unified view; account details and statements; NEFT/RTGS/IMPS funds transfer; utility payments; requirements, process, UX and test planning for these capabilities.

### Out of scope / not yet defined

Home-loan and mutual-fund journeys; product application/onboarding and KYC; card issuance; dispute/chargeback; lending decisions; investment advice/trading; branch systems; full contact-centre tooling; exact mobile/web channel; production architecture and vendor selection. Revisit after release planning.

## 6. Assumptions to validate

- Retail customers are the primary end users.
- A customer may have one or more eligible accounts and/or cards.
- Existing bank systems expose account, card, statement, and payment services through approved interfaces.
- The final release plan will be approved by the managing committee/project team.
- A named policy owner will provide payment, authentication, data, and exception rules.

## 7. Constraints, dependencies and risks

See [source notes and decisions](14_Source_Notes_and_Decisions.md). Critical risks include wrong institution naming, undecided release sequencing, unspecified payments controls, integration uncertainty, customer eligibility edge cases, and lack of approved non-functional requirements.

## 8. Benefits and measures

| Benefit hypothesis | Candidate measure | Baseline/target |
|---|---|---|
| More customers self-serve | Share of eligible servicing tasks completed digitally | To establish |
| Faster access to information | Time to retrieve account/card details and statements | To establish |
| Fewer avoidable contacts | Contact volume for in-scope tasks | To establish |
| More reliable payments | Completion, failure, duplicate, and reversal rates by transaction type | To establish with operations |
| Better task comprehension | Customer task completion and error rate in usability testing | To establish |

No benefit realization or ROI result is claimed.
