# Software Requirements Specification (SRS)

**Status:** High-level draft; engineering, security, data, and operations review required.

## 1. Purpose and scope

Describe candidate software behavior for a digital retail-banking application supporting banking and credit-card self-service. See [FRD](05_FRD_and_RTM.md) for functional requirements and [baseline](00_Project_Baseline.md) for scope boundaries.

## 2. User classes

- Retail customer with one or more bank products.
- Operations/support user (only if a staff-facing capability is approved; otherwise support is external to this app).
- System/service actors: identity, core banking, card, payment, and utility services (illustrative only).

## 3. Interfaces to define

- User interface: mobile, web, or both — decision pending.
- External/system interfaces: identity, core banking, card processing, payment rails, utility/biller services, support channel — existence and contracts unconfirmed.
- Communication interfaces: secure API and event/status mechanisms to be agreed by architecture and security.

## 4. Functional system requirements

See FR-01 through FR-14 in the [FRD](05_FRD_and_RTM.md). These include sign-in, product summary, account/card details, statements, transfer and utility payment initiation, card balance payment, safe status presentation, support routing, error handling, and audit events.

## 5. Non-functional requirement catalogue (targets TBD)

| ID | Quality area | Requirement to baseline |
|---|---|---|
| NFR-01 | Security | Define approved authentication, authorization, session, encryption, secrets, monitoring, and secure development controls. |
| NFR-02 | Privacy | Minimize exposed personal/financial data; define consent, masking, retention, and access rules. |
| NFR-03 | Availability | Set service hours/availability objectives and graceful degradation behavior. |
| NFR-04 | Performance | Define response-time targets for sign-in, summary, statement retrieval, and transaction submission/status. |
| NFR-05 | Reliability | Define idempotency, retry, timeout, reconciliation, and recovery behavior for transactions. |
| NFR-06 | Accessibility | Agree accessibility standard, assistive-technology support, and verification method. |
| NFR-07 | Compatibility | Define supported devices, OS/browser versions, network conditions, and localization. |
| NFR-08 | Auditability | Define auditable events, timestamps, identifiers, protected logs, and retention. |
| NFR-09 | Usability | Define task-completion and comprehension targets for priority journeys. |
| NFR-10 | Maintainability | Define supportability, observability, configuration, and release requirements. |

No numeric NFR targets are invented in this document.

## 6. Data requirements

Candidate entities include Customer, Account, Card, Bank Statement, Card Statement, Payment/Transfer, Biller, and Transaction Status. Define data owner, authoritative source, field-level classification, masking, retention, freshness, reconciliation, and deletion/archival requirements.

## 7. Error and transaction behavior

Transaction flows must distinguish validation failure before submission from an uncertain outcome after submission. For a timeout, the interface should query or display authoritative status and avoid encouraging a potentially duplicate resubmission. Exact mechanisms and state model are architecture decisions.

## 8. Verification

Functional requirements map to UAT cases in [UAT plan](13_UAT_Plan.md). Security, performance, accessibility, integration, recovery, and operational-readiness testing must be added after approved NFRs and interface contracts are available.
