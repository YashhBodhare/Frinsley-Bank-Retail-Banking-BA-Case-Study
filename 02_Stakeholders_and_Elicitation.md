# Stakeholders and Elicitation Plan

## Stakeholder register (candidate list)

| Stakeholder / role | Interest and likely contribution | Influence | Engagement approach | Evidence status |
|---|---|---:|---|---|
| Managing committee / sponsor | Approves launch sequencing, strategic outcomes, investment envelope | High | Decision workshop; confirm success measures and release gates | Role implied by source; names/decisions absent |
| Product owner | Owns backlog, scope, prioritisation, stakeholder alignment | High | Weekly refinement; decision log; acceptance review | Source says PO meetings have begun |
| Retail banking customers | Need clear account, statement, transfer and payment journeys | Medium | Interviews/usability sessions; accessible survey | Candidate user group |
| Credit-card customers | Need card details, statement access, balance payment | Medium | Interviews and task testing | Candidate user group |
| Branch/contact-centre operations | Explain current servicing, exceptions, support and customer pain points | High | Process walkthrough and exception workshop | Candidate role |
| Payments operations | Validate transfer rail handling, limits, status, reconciliation, reversals | High | Rule-focused workshop | Candidate role |
| Card operations | Validate statement lifecycle, card status, payment allocation and exceptions | High | Process and data workshop | Candidate role |
| Technology partner / engineering | Assess architecture, APIs, feasibility, non-functional requirements | High | Technical discovery and story refinement | Partner development source fact; named team unknown |
| Information security / fraud | Define authentication, authorization, monitoring, device/session and fraud controls | High | Threat/control review | Candidate roles; no controls supplied |
| Risk / compliance / legal | Validate applicable obligations, disclosures, records, complaints and approvals | High | Control and policy review | Candidate roles; no jurisdiction/policy supplied |
| UX / accessibility | Convert requirements into usable, accessible journeys | Medium | Co-design and prototype testing | Candidate role |
| Utility / payment partners | Validate biller catalogue, payment response, settlement and failure handling | Medium | Integration discovery | Dependency hypothesis |

## Power-interest view (initial hypothesis)

|  | Higher interest | Lower / uncertain interest |
|---|---|---|
| **Higher influence** | Sponsor/committee, product owner, payments & card operations, technology, security, risk/compliance | Executive functions not yet identified; keep informed once mapped |
| **Lower influence** | Retail customers, branch/contact-centre staff, UX/accessibility contributors | External utility/payment partners until integration scope is agreed |

This is a starting hypothesis only. Reassess after interviews; stakeholder influence and interest were not supplied in the source.

## Elicitation objectives

1. Confirm release 1 boundaries and how the committee’s launch plan affects both modules.
2. Define customer, account, card, and role eligibility.
3. Detail data shown in unified view, account/card details, and statement views.
4. Specify payment/transfer rules, controls, lifecycle statuses, exceptions, and support hand-offs.
5. Identify integration, security, privacy, audit, accessibility, channel, and performance needs.
6. Agree measurable business and customer outcomes.

## Planned methods and outputs

| Method | Participants | Focus | Output |
|---|---|---|---|
| Document review | PO, operations, compliance, technology | Product policies, statement samples, payment procedures, architecture constraints | Source register and requirements baseline |
| Semi-structured interviews | Customer, operations, product, control functions | Goals, current workarounds, edge cases, decision rights | Interview notes, validated needs, open questions |
| Process walkthrough | Payments/card operations, support | Current steps, hand-offs, systems, failure paths | Validated As-Is map and control points |
| Facilitated scope workshop | Sponsor, PO, operations, technology | MVP, release sequencing, MoSCoW, dependencies | Signed scope decisions and backlog |
| Prototype/usability sessions | Representative customers, UX | Discoverability, comprehension, task success, error recovery | Findings, prioritized design changes |
| Requirements review | PO, SMEs, delivery, QA | Clarity, atomicity, feasibility, testability, traceability | Approved baseline or comments log |

## Interview prompts

- Which customers and accounts may access the digital service? How are joint, business, blocked, dormant, or closed accounts handled?
- What is the authoritative source for balances, card state, statement data, and transaction status?
- Which fields must appear in the unified view? How fresh must each field be?
- What are the exact definitions of “current”, “last”, and “detailed” statement?
- Which transfer types, destinations, limits, charges, cut-offs, approvals, and confirmation steps apply?
- How are new beneficiaries, failed/duplicate requests, reversals, and pending transactions handled?
- Which utility billers and payment confirmation semantics are in scope?
- How is a card payment funded, allocated, scheduled, and confirmed? Are partial/overpayments supported?
- What authentication, step-up verification, fraud monitoring, and audit requirements apply?
- What accessibility, localization, support, availability, and performance standards are required?

## Elicitation record status

The presentation says stakeholder meetings have started but supplies no participants, dates, minutes, findings, or decisions. The methods above are a plan and must not be described as completed research.
