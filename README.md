# Frinsley Bank — Retail Banking BA Case Study

An end-to-end Business Analysis case study for a proposed digital retail-banking application. The project brief covers credit-card servicing and banking self-service, including statements, transfers, utility payments, and card-balance payments.

> **Project name:** Frinsley Bank (spelled F-R-I-N-S-L-E-Y), as confirmed by the project owner and shown in the supplied presentation.

## Project overview

| Area | Summary |
|---|---|
| Business context | Newly licensed bank preparing phased product launches |
| Proposed solution | Retail banking software application developed with a technology partner |
| Credit-card module | Card details, current and previous statements, detailed statement, balance payment |
| Banking module | Login, unified view, account details and statements, NEFT/RTGS/IMPS transfers, utility payments |
| Broader services mentioned | Home loans and mutual funds; detailed functionality was not provided in the brief |
| BA work | Requirements, stakeholders, stories, wireframes, process models, BRD/PRD/FRD/SRS, gap and solution analysis, UAT planning |

## Start here

- [Project baseline and scope](00_Project_Baseline.md)
- [BA capability matrix](01_Capability_Matrix.md)
- [Stakeholders and elicitation plan](02_Stakeholders_and_Elicitation.md)
- [Stakeholder questionnaire](03_Stakeholder_Questionnaire.md)
- [BRD — Business Requirements Document](04_BRD.md)
- [FRD and Requirements Traceability Matrix](05_FRD_and_RTM.md)
- [Epics, user stories, and acceptance criteria](06_User_Stories.md)
- [Wireframe specifications](07_Wireframe_Specifications.md)
- [Process maps](08_Process_Maps.md)
- [Models, BPMN, and Miro board plan](09_Models_BPMN_and_Miro.md)
- [PRD — Product Requirements Document](10_PRD.md)
- [SRS — Software Requirements Specification](11_SRS.md)
- [Gap analysis and solution mapping](12_Gap_Analysis_and_Solution_Mapping.md)
- [UAT plan](13_UAT_Plan.md)
- [Source notes, assumptions, and decisions](14_Source_Notes_and_Decisions.md)

## Wireframes and prototype

The project includes eight visual mobile wireframes and one click-through prototype. The gallery previews the individual SVG screens; the prototype brings the main journeys together in one browser file.

- [Open the full wireframe gallery](wireframes/README.md)
- [Open the click-through prototype](wireframes/prototype.html)
- [Sign-in screen](wireframes/01-sign-in.svg) · [Unified overview](wireframes/02-unified-overview.svg) · [Account and statements](wireframes/03-account-and-statements.svg)
- [Transfer details](wireframes/04-transfer-details.svg) · [Transfer review and status](wireframes/05-transfer-review-status.svg) · [Card details and statements](wireframes/06-card-details-statements.svg)
- [Card payment](wireframes/07-card-payment.svg) · [Utility payment](wireframes/08-utility-payment.svg)

<details>
<summary>Preview all eight wireframe screens in this README</summary>

### Sign-in
![Frinsley Bank sign-in wireframe](wireframes/01-sign-in.svg)

### Unified overview
![Frinsley Bank unified overview wireframe](wireframes/02-unified-overview.svg)

### Account and statements
![Frinsley Bank account and statements wireframe](wireframes/03-account-and-statements.svg)

### Transfer details
![Frinsley Bank transfer details wireframe](wireframes/04-transfer-details.svg)

### Transfer review and status
![Frinsley Bank transfer review and status wireframe](wireframes/05-transfer-review-status.svg)

### Card details and statements
![Frinsley Bank card details and statements wireframe](wireframes/06-card-details-statements.svg)

### Card payment
![Frinsley Bank card payment wireframe](wireframes/07-card-payment.svg)

### Utility payment
![Frinsley Bank utility payment wireframe](wireframes/08-utility-payment.svg)

</details>

To run the prototype, download or clone the repository and open [`wireframes/prototype.html`](wireframes/prototype.html) in a browser. Its interactions are illustrative: it does not authenticate users, connect to bank services, or submit transactions.

## Evidence and status labels

- **Source fact** — explicitly stated in the supplied project presentation.
- **Analyst draft** — a proposed requirement, workflow, acceptance criterion, or design created to make the case study reviewable; it is not approved bank policy.
- **To validate** — requires confirmation from a product, operations, technology, security, risk, or compliance stakeholder.
- **Not evidenced** — the supplied brief does not establish that the activity occurred or that the result is real.

No interviews, survey responses, approvals, production results, or executed UAT outcomes are represented as completed. The user stories, wireframes, process flows, models, gap analysis, solution options, and UAT scenarios are analyst drafts based on the supplied brief.

## Suggested GitHub repository details

**Repository title:** `Frinsley Bank Retail Banking BA Case Study`  
**Description:** `End-to-end BA case study for Frinsley Bank's proposed retail banking app, covering credit cards, account servicing, transfers, utility payments, requirements, process models, wireframes, and UAT planning.`  
**Suggested repository slug:** `frinsley-bank-retail-banking-ba-case-study`

## Scope note

The supplied presentation includes home loans and mutual funds as bank services, but it does not give detailed requirements for them. They are treated as future scope candidates, not as designed modules in this case study. The source’s banking slide appears to carry over a credit-card heading; the issue and interpretation are recorded in [source notes and decisions](14_Source_Notes_and_Decisions.md).

## Use of this case study

This is a learning and portfolio artifact, not a live banking specification or implementation instruction. Banking controls, transaction rules, accessibility, security, privacy, records retention, channel scope, and applicable obligations must be determined and approved by the relevant specialists before delivery.
