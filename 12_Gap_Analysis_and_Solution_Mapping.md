# Gap Analysis and Solution Mapping

**Evidence limitation:** Detailed current procedures were not supplied. The current-state column below records known capability gaps or explicit unknowns, not validated operational findings.

## Gap analysis

| Area | Current evidence / gap | Target capability | Proposed response | Priority / validation |
|---|---|---|---|---|
| Product access | New bank; digital access details unknown | Authorized sign-in and product-specific access | Define identity, eligibility, account/card authorization | Must; security/product review |
| Unified view | Not specified | Customer can navigate eligible accounts and cards in one place | Establish product summary and freshness contract | Must; product/data review |
| Statements | Feature named; periods/format unclear | Current/previous/detailed views with clear availability | Define statement catalogue, data source and presentation | Must; operations/card review |
| Transfers | NEFT/RTGS/IMPS named; rules absent | Validated, reviewable, controlled transfer with reliable status | Specify rail rules, limits, fees, cut-offs, status, idempotency | Must; payments/security review |
| Utility payments | Feature named; billers and failures absent | Select biller, provide details, confirm and track result | Confirm provider list, validation and payment lifecycle | Should; payments/partner review |
| Card payment | Balance payment named; amount/source/allocation rules absent | Review and initiate eligible payment with clear outcome | Define funding source, amount options, due-date timing, allocation | Must; card/payments review |
| Exceptions/support | No process supplied | Safe and understandable recovery/support route | Define pending, failed, timeout, reversal, and support flows | Must; operations/technology review |
| Controls/NFRs | Policies and targets absent | Approved security, privacy, audit, accessibility, availability and performance | Run control discovery and baseline NFRs | Must; specialist approval |
| Release sequencing | Committee to decide launch plan | Scope synchronized with business launch | Decision workshop and dependency-based release plan | Blocking decision |

## Candidate solution options

| Option | Description | Benefits | Trade-offs / risks | Assessment |
|---|---|---|---|---|
| A. Single integrated digital application | Banking and card modules in one customer experience, backed by approved domain services | Unified navigation, shared access patterns, coherent customer view | Higher integration and release coordination; data freshness and failure isolation need design | Candidate direction; architecture feasibility review |
| B. Separate banking and card journeys with shared access | Distinct domain modules under common sign-in/navigation | Domain teams can own focused journeys; staged rollout may be easier | Inconsistent experience/data presentation; shared identity and hand-off complexity | Consider if release ownership or service constraints require separation |
| C. Manual-assisted digital entry | Digital application supports discovery/forms while staff complete some operations | May support staged capability where integrations are unavailable | More hand-offs and delays; customer expectation and reconciliation risks | Temporary fallback only if approved; assess operational capacity |

No option is approved. Score after stakeholder discovery against customer value, control fit, feasibility, integration effort, operational readiness, cost, time, reliability, accessibility, and maintainability.

## Solution mapping (need → capability → story → verification)

| Need | Capability | Story | Requirements | Verification |
|---|---|---|---|---|
| Securely access products | Sign-in and authorization | US-01 | FR-01 | UAT-01, 02; security tests TBD |
| See products together | Unified view | US-02 | FR-02 | UAT-02 |
| Review bank activity | Account and statement views | US-03, US-04 | FR-03, FR-04 | UAT-03–05 |
| Transfer funds | Transfer prepare/review/status | US-05–US-07 | FR-05–FR-07 | UAT-06–09 |
| Pay a bill | Biller and payment flow | US-08 | FR-08 | UAT-12–13 |
| Manage card activity | Card details and statement | US-09 | FR-09, FR-10 | UAT-10–11 |
| Pay card balance | Card payment flow | US-10 | FR-11 | UAT-15 |
| Resolve service issue | Help and safe error recovery | US-11 | FR-12–FR-14 | UAT-14; support validation |

## Root-cause analysis plan

Once validated pain points are collected, use 5 Whys/fishbone or service blueprinting to separate policy, process, data, integration, access, training, and usability causes. No root cause is asserted from the supplied deck alone.
