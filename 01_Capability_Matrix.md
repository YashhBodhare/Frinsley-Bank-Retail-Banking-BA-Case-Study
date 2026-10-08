# BA Capability Matrix — Frinsley Bank

The matrix maps the portfolio website’s four capability groups to the case-study evidence in this repository. “Covered” means a draft artifact is provided; it does not mean a real-world activity was performed or approved.

## Coverage key

- **Source** — the source deck explicitly mentions the item.
- **Draft** — the artifact is constructed from the brief for portfolio demonstration.
- **Plan** — approach/template supplied; activity or outcome is not evidenced.
- **Validate** — subject-matter confirmation required.

## Core BA capabilities

| Website capability | Bank case application | Evidence / location | Status |
|---|---|---|---|
| Stakeholder Analysis | Identify decision-makers, users, delivery roles, control functions, and partner dependencies | [Stakeholder register](02_Stakeholders_and_Elicitation.md) | Draft / validate |
| Requirements Elicitation | Structure interviews, workshops, questionnaires, and document review around the two modules | [Elicitation plan](02_Stakeholders_and_Elicitation.md), [questionnaire](03_Stakeholder_Questionnaire.md) | Plan; meetings noted in source, findings not supplied |
| Requirements Analysis | Decompose features into requirements, rules, exceptions, and traceability links | [FRD and RTM](05_FRD_and_RTM.md) | Draft |
| Process Improvement | Compare a clearly labeled current-state hypothesis with proposed digital flows and identify control/experience opportunities | [Process maps](08_Process_Maps.md), [gap analysis](12_Gap_Analysis_and_Solution_Mapping.md) | Draft / validate |
| Solution Evaluation | Compare solution options against customer needs, operational fit, risk, integration, and testability | [Solution mapping](12_Gap_Analysis_and_Solution_Mapping.md) | Draft; no vendor evaluation performed |
| Business Case Development | Frame expected value, cost categories, assumptions, dependencies, and benefits measures for the sponsor to validate | [BRD](04_BRD.md), [PRD](10_PRD.md) | Outline only; financial case not evidenced |

## Techniques and methods

| Technique | Application | Evidence | Status |
|---|---|---|---|
| Stakeholder Interviews | Role-based questions for product, operations, payments, cards, security, compliance, and customers | [Elicitation plan](02_Stakeholders_and_Elicitation.md) | Planned; no transcripts/results supplied |
| 5 Whys | Investigate validated pain points such as unclear transaction status or fragmented servicing | [Gap analysis](12_Gap_Analysis_and_Solution_Mapping.md) | Candidate technique; root cause unverified |
| MoSCoW Prioritisation | Initial release priorities across source features | [User stories](06_User_Stories.md) | Provisional, pending product decision |
| Gap Analysis | Contrast source/current-state hypothesis with target capabilities | [Gap analysis](12_Gap_Analysis_and_Solution_Mapping.md) | Draft |
| Facilitated Workshops | Resolve release scope, payment rules, statement definitions, and exception handling | [Elicitation plan](02_Stakeholders_and_Elicitation.md) | Planned; workshops not evidenced |
| Root-Cause Analysis | Classify process, policy, data, integration, and channel causes once evidence is gathered | [Gap analysis](12_Gap_Analysis_and_Solution_Mapping.md) | Framework supplied; findings pending |

## BA deliverables

| Deliverable | Case-study evidence | Status |
|---|---|---|
| Business Requirements Document | [BRD](04_BRD.md) | Analyst draft |
| User Stories | [Epics and stories](06_User_Stories.md) | Analyst draft; no Jira records created |
| Acceptance Criteria | Included per story in [user stories](06_User_Stories.md) | Analyst draft |
| Requirements Traceability Matrix | [FRD and RTM](05_FRD_and_RTM.md) | Analyst draft |
| Business Rules | [FRD](05_FRD_and_RTM.md) and [decisions](14_Source_Notes_and_Decisions.md) | Candidate rules marked for approval |
| UAT Scenarios | [UAT plan](13_UAT_Plan.md) | Planned; no execution/results claimed |

## Models and diagrams

| Model or diagram | Case-study evidence | Status |
|---|---|---|
| As-Is Process Map | [Process maps](08_Process_Maps.md) | Explicit current-state hypothesis only; validate with operations |
| To-Be Process Map | [Process maps](08_Process_Maps.md) | Draft target flows |
| BPMN Diagram | [Models and BPMN](09_Models_BPMN_and_Miro.md) | Conceptual Mermaid BPMN-style draft; formal BPMN 2.0 validation needed |
| Use-Case Diagram | [Models and BPMN](09_Models_BPMN_and_Miro.md) | Draft |
| Stakeholder Map | [Stakeholder register](02_Stakeholders_and_Elicitation.md) | Text power-interest map; validate influence/interest |
| Wireframe | [Wireframe gallery](wireframes/README.md), [click-through prototype](wireframes/prototype.html), and [specifications](07_Wireframe_Specifications.md) | Visual low-fidelity draft; not approved UI |

## Overall evidence statement

The source presentation explicitly contains the business context, two module feature lists, expected presentation deliverables, and the fact that stakeholder meetings have started. The detailed analysis artifacts in this pack are portfolio drafts built from those facts. See [source notes and decisions](14_Source_Notes_and_Decisions.md) before publishing claims about research or project outcomes.
