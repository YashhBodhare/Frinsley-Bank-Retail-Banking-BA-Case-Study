# Functional Requirements Document (FRD) and Requirements Traceability Matrix

**Status:** Analyst draft. Functional behavior and banking policies require owner approval.

## 1. Functional requirements

| ID | Module | Functional requirement | Priority | Validation note |
|---|---|---|---|---|
| FR-01 | Access | The system shall authenticate a customer using the bank-approved sign-in method. | Must | Define credentials, MFA/step-up, recovery, lockout, session rules |
| FR-02 | Unified view | The system shall present the signed-in customer’s eligible accounts and cards in a consolidated view. | Must | Define eligibility, ordering, freshness, unavailable-data state |
| FR-03 | Account details | The customer shall be able to open an account and view approved account details. | Must | Confirm fields, masked identifiers, account statuses |
| FR-04 | Bank statements | The customer shall be able to select and view available bank statements. | Must | Define periods, formats, access history, download/print |
| FR-05 | Transfer | The customer shall be able to select a supported transfer type (NEFT, RTGS, IMPS) and enter/choose the required destination and amount. | Must | Validate rail-specific data, limits, fee, cut-off, eligible destinations |
| FR-06 | Transfer review | Before submission, the system shall show a review of the transfer details and request any required confirmation/authentication. | Must | Validate disclosure and security policies |
| FR-07 | Transfer outcome | The system shall display a transaction reference and a bank-defined status after submission, including safe handling of timeout/pending outcomes. | Must | Status values and reconciliation contract needed |
| FR-08 | Utility payment | The customer shall be able to select an available biller, provide required billing details, review, and submit a supported payment. | Should | Biller list, validation, fees, receipt and failure handling needed |
| FR-09 | Card details | The customer shall be able to view approved details for an eligible credit card. | Must | Define masking and status/limits/available-credit fields |
| FR-10 | Card statements | The customer shall be able to open the current-period, previous-period, and detailed statement views where available. | Must | Clarify “last statement” and detailed transaction scope |
| FR-11 | Card payment | The customer shall be able to initiate a card balance payment from an approved funding source and review it before submission. | Must | Define amounts, allocation, due-date rules, timing and outcomes |
| FR-12 | Support | The system shall provide an approved support route when the customer cannot complete an in-scope task. | Should | Source does not specify support feature; validate channels/hours |
| FR-13 | Error handling | The system shall explain validation errors and next steps without exposing sensitive information. | Must | Copy, security and accessibility review required |
| FR-14 | Audit | The system shall record access and transaction events required by approved bank policy. | Must | Define event schema, retention and access controls |

## 2. Candidate business rules

| Rule ID | Draft rule | Owner to validate |
|---|---|---|
| RULE-01 | A user may view only accounts and cards for which the bank has authorized that user. | Identity/access, product, compliance |
| RULE-02 | A transfer cannot be submitted until required fields and applicable control checks pass. | Payments, security, risk |
| RULE-03 | The interface must not show a transfer as successful solely because the customer tapped Submit; it must use an authoritative response/status. | Payments/technology |
| RULE-04 | Sensitive identifiers must be masked according to bank policy. | Security/privacy/product |
| RULE-05 | The customer may initiate card payment only from funding sources permitted by bank policy. | Card/payments |

## 3. RTM (high-level)

| Business req | Functional reqs | Story IDs | Process / design | UAT scenarios |
|---|---|---|---|---|
| BR-02 | FR-01, FR-02, FR-12 | US-01, US-02, US-11 | Login; unified view | UAT-01, 02, 14 |
| BR-03 | FR-03, FR-04, FR-09, FR-10 | US-03, US-04, US-08, US-09 | Account/card details; statement flows | UAT-03–05, 10–11 |
| BR-04 | FR-05–FR-07, FR-13–FR-14 | US-05–US-07 | Transfer initiation and status | UAT-06–09 |
| BR-05 | FR-08, FR-13–FR-14 | US-07 | Utility payment | UAT-12–13 |
| BR-06 | FR-11, FR-13–FR-14 | US-10 | Card payment | UAT-12, 15 |
| BR-08 | FR-01, FR-06–FR-07, FR-11, FR-13–FR-14 | US-01, US-05–US-11 | Authentication and transaction controls | UAT-01, 07–09, 13–15 |

## 4. Requirement quality checklist

Before baseline approval, confirm each requirement is atomic, unambiguous, feasible, necessary, implementation-neutral where appropriate, measurable/testable, assigned an owner, prioritized, and linked to an approved source or decision. Add version, change history, approver, and effective date in Jira/requirements tooling.
