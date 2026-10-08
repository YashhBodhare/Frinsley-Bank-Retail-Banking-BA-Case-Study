# Models, BPMN, and Miro Board Plan

All models below are analyst drafts derived from the short brief. Confirm role boundaries, systems, and policy with stakeholders before treating them as baseline.

## Context / system boundary

```mermaid
flowchart LR
 C[Retail customer] --> A[Digital banking application]
 A --> Core[Core banking services]
 A --> Card[Card services]
 A --> Pay[Payment and utility services]
 A --> Support[Customer support]
```

Candidate integrations are illustrative. The source does not name systems or establish that these interfaces exist.

## Use-case view

```mermaid
flowchart TD
 Customer[Retail customer] --> UC1[Sign in and view unified products]
 Customer --> UC2[View account and bank statement]
 Customer --> UC3[Initiate transfer or utility payment]
 Customer --> UC4[View card statement and pay balance]
 Ops[Operations / support] --> UC5[Resolve service exception]
```

## Conceptual data model (draft)

```mermaid
erDiagram
 CUSTOMER ||--o{ ACCOUNT : authorized_for
 CUSTOMER ||--o{ CARD : authorized_for
 ACCOUNT ||--o{ BANK_STATEMENT : has
 CARD ||--o{ CARD_STATEMENT : has
 ACCOUNT ||--o{ PAYMENT : funds
 CARD ||--o{ PAYMENT : receives
 PAYMENT }o--|| TRANSACTION_STATUS : has
```

The diagram conveys conceptual entities only; it is not a database design. Data ownership, joint access, retention, PII fields, cardinalities, and payment types require data-owner/security review.

## BPMN-style transfer process

```mermaid
flowchart TD
 S((Start)) --> T[Select rail and enter details]
 T --> G{Validation and controls pass?}
 G -- No --> E[Show correction or rejection]
 E --> T
 G -- Yes --> R[Review details and confirm]
 R --> P[Submit to payment service]
 P --> X{Service response}
 X -- Accepted --> A[Show status and reference]
 X -- Pending or timeout --> Q[Show pending state and safe next step]
 X -- Rejected --> N[Show rejection and help route]
 A --> F((End))
 Q --> F
 N --> F
```

This is BPMN-inspired Mermaid, not an exported BPMN 2.0 model. Formal BPMN should identify pools/lanes, message flows, events, gateways, exception boundaries, and system ownership in an appropriate modeling tool.

## Miro board layout

1. **Frame 1 — Charter:** problem, objectives, scope, constraints, open questions.
2. **Frame 2 — Stakeholders:** role map, power/interest, decision owners.
3. **Frame 3 — Research:** interview plan, evidence wall, validated facts vs assumptions.
4. **Frame 4 — Journey and As-Is:** one frame per transfer, utility payment, card payment; mark unknowns.
5. **Frame 5 — To-Be:** customer journey, backstage operations, systems, exception routes.
6. **Frame 6 — Requirements:** epics, story cards, business rules, priorities, trace links.
7. **Frame 7 — Risks and decisions:** payment controls, access, data, integration, release dependencies.
8. **Frame 8 — Validation:** review owners, UAT scenario links, decision/action register.

Use consistent sticky-note colors for source facts, analyst assumptions, validation questions, and approved decisions; include owner and date on each decision.
