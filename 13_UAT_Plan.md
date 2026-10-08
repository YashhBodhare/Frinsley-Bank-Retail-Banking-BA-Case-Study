# User Acceptance Testing (UAT) Plan

**Status:** Draft test scenarios; no UAT execution or pass results are claimed.

## UAT objectives

Confirm that approved business requirements and customer journeys work as expected for eligible users, including success, validation, exception, status, and support paths. UAT should use bank-approved test data and environments; never use real customer financial data in an uncontrolled environment.

## Entry criteria

- Product/release scope, business rules, acceptance criteria, interface behavior, and test environment approved.
- Test accounts/cards and payment/biller simulators or approved test services available.
- Authentication, roles, data masking, expected transaction outcomes, and support contacts defined.
- Critical defects from system/integration testing resolved or formally accepted.

## Exit criteria

- All Must-priority scenarios executed with outcomes recorded.
- No unresolved critical/high-severity defects unless an authorized business owner accepts them with a documented workaround/risk.
- Traceability and evidence attached; business/product owners record approval or rejection.

## Scenario catalogue

| ID | Scenario | Expected result | Trace |
|---|---|---|---|
| UAT-01 | Sign in with valid credentials and required verification | Authorized customer reaches home view | FR-01, US-01 |
| UAT-02 | Attempt sign-in with invalid/locked credentials | Safe error and approved recovery; no product data exposed | FR-01, US-01 |
| UAT-03 | Open an eligible account from unified view | Approved details appear with masking | FR-02, FR-03, US-02/03 |
| UAT-04 | Open an available bank statement | Correct period and statement display | FR-04, US-04 |
| UAT-05 | Request unavailable statement period | Clear unavailable state and approved next step | FR-04, FR-13 |
| UAT-06 | Prepare valid transfer on an enabled rail | Required details validate and review screen is accurate | FR-05/06, US-05/06 |
| UAT-07 | Submit transfer that fails an approved rule | Request is blocked with useful reason; no transfer created | FR-05/06, US-05/06 |
| UAT-08 | Submit valid transfer with authoritative completed response | Accurate completed status and reference shown | FR-07, US-06/07 |
| UAT-09 | Transfer receives pending/timeout response | Pending/unknown state shown; safe status-check path; no duplicate created | FR-07, US-07 |
| UAT-10 | View eligible card details | Approved masked card data shown | FR-09, US-09 |
| UAT-11 | View current, previous, and detailed card statements | Correct approved statement view selected | FR-10, US-09 |
| UAT-12 | Submit valid utility payment for an enabled biller | Review, confirmation, status and reference are correct | FR-08, US-08 |
| UAT-13 | Utility provider unavailable or rejects request | No false success; clear recovery/support path | FR-08, FR-13, US-07/08 |
| UAT-14 | Trigger relevant service error and choose help | Approved support route and contextual guidance appear | FR-12/13, US-11 |
| UAT-15 | Initiate valid card balance payment | Review and authoritative payment outcome are correct | FR-11, US-10 |

## Execution record template

For each case record: tester, date, build/environment, preconditions, test data reference, steps, expected result, actual result, Pass/Fail/Blocked, evidence link, defect ID/severity, retest result, and business sign-off. Security, performance, accessibility, recovery, and regulatory/control tests require separate approved plans and are not replaced by this UAT list.
