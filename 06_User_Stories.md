# Epics, User Stories, and Acceptance Criteria

Stories are **analyst drafts**. Initial MoSCoW values are provisional. Story points, assignees, sprint commitments, and Jira statuses are intentionally left blank until estimation and team planning.

## Epic E-01 — Secure access and unified view

### US-01 — Sign in securely
**As a** retail customer, **I want** to sign in using the bank-approved method, **so that** I can access my eligible banking services securely.  
**Priority:** Must · **Estimate/owner/status:** TBD

- Given valid credentials and required verification, when I complete sign-in, then I reach the authorized home view.
- Given invalid credentials, when sign-in fails, then I receive a safe, accessible message and a permitted recovery route.
- Given my account is locked or temporarily unavailable, then the system explains the next approved step without disclosing sensitive account data.

### US-02 — View a unified account and card summary
**As a** signed-in customer, **I want** to see my eligible accounts and cards together, **so that** I can choose the service I need.

- The view contains only products I am authorized to access.
- Each item displays the approved summary fields and a clear route to its details.
- If one data source is unavailable, the system identifies what is unavailable and does not present stale data as current.

## Epic E-02 — Bank account information

### US-03 — View account details
**As a** customer, **I want** to open an account and see its approved details, **so that** I can identify and understand the account.

- Account identifiers are masked according to policy.
- Status, currency, and other fields match the approved account data contract.
- Unauthorized or unavailable accounts are not exposed.

### US-04 — View bank statements
**As a** customer, **I want** to select an available statement period, **so that** I can review account activity.

- Available statement periods are clearly listed.
- Selecting a period opens the corresponding statement or a helpful unavailable state.
- Any download/print feature appears only if approved and preserves required access controls.

## Epic E-03 — Transfers and utility payments

### US-05 — Prepare a bank transfer
**As a** customer, **I want** to choose an available transfer type and enter transfer details, **so that** I can move money using an approved payment rail.

- Only currently supported transfer types are selectable.
- Required details and validation rules are rail-specific and approved.
- The amount, destination, applicable charges, and timing disclosures are visible before confirmation as required by policy.

### US-06 — Review and submit transfer
**As a** customer, **I want** to review and confirm a transfer, **so that** I can detect errors before submitting it.

- A review screen shows the destination, amount, transfer type, fees if any, and other approved details.
- Required authentication/confirmation is completed before submission.
- Repeated taps or retry behavior do not create duplicate transfers unless the bank’s authoritative status confirms the first attempt was not accepted.

### US-07 — Check transfer or utility payment status
**As a** customer, **I want** to see the bank-reported status and reference for a submitted payment, **so that** I know what happened and what to do next.

- The status comes from the authoritative transaction service.
- Pending, completed, rejected, and unknown/timeout outcomes have distinct approved messaging.
- A reference is shown when available; the customer is not instructed to retry in a way that could duplicate a pending transaction.

### US-08 — Pay a utility bill
**As a** customer, **I want** to select an available biller and submit a bill payment, **so that** I can pay an eligible utility from the digital channel.

- The customer can find/select only available billers.
- Billing details are validated before submission.
- The customer reviews the payment and sees the authoritative status and receipt/reference when available.

## Epic E-04 — Credit-card servicing

### US-09 — View card details and statements
**As a** cardholder, **I want** to see my eligible card details and current/previous/detailed statements, **so that** I can understand my card activity and balance.

- Only authorized cards are displayed and sensitive card data is masked.
- Current, previous (“last”), and detailed statement options are clearly distinguished once business definitions are approved.
- Unavailable statements show an explanation and support route.

### US-10 — Pay credit-card balance
**As a** cardholder, **I want** to initiate a payment toward my card balance, **so that** I can manage my outstanding amount.

- Available payment amounts/funding sources follow approved rules.
- The review step shows the selected card, amount, funding source, and any required timing/disclosure.
- The final status and reference reflect the authoritative payment response.

## Epic E-05 — Help and service recovery

### US-11 — Get help for an in-scope task
**As a** customer, **I want** an approved help option when I encounter an issue, **so that** I can resolve it without guessing.

- Help is available from relevant failure or unavailable states.
- Contact options, hours, and information to prepare are approved by operations.
- Support guidance does not expose protected information.

## Backlog refinement fields (Jira-ready)

For each story, add: issue type; epic link; requirement ID; priority; points after team estimation; owner after staffing; workflow status; dependencies; labels (banking/cards/payments/control); acceptance criteria; UX/design link; test/UAT IDs; decision links. No assignments or estimates are asserted in this draft.
