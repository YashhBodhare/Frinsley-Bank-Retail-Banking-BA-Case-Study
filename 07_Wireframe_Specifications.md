# Wireframe Specifications

Visual deliverables now accompany these specifications: see [the wireframe gallery](wireframes/README.md) for eight GitHub-renderable SVG screens and [the clickable prototype](wireframes/prototype.html) for a local browser walkthrough. They are low-fidelity analyst drafts, not final visual designs. UX and accessibility teams should validate information hierarchy, navigation, responsive behavior, and content.

## WF-01 Sign-in

- Bank identity and accessible sign-in heading.
- Approved credential fields, show/hide behavior if permitted, recovery route, verification step, support/help link.
- Inline field validation; safe generic failure messages; loading, locked, and unavailable states.
- No sensitive account data before successful authorization.

## WF-02 Unified home

- Header: greeting, support, profile/security actions.
- Account cards and credit-card summaries, each showing only approved masked identifiers and selected summary values.
- Entry points: Accounts, Transfers, Utility payments, Cards, Statements.
- Data freshness indicator and partial-service warning where required.
- Empty state for no eligible products; system error state with recovery/support.

## WF-03 Account details and statement list

- Account title and masked number, approved status and balance fields.
- Statement list grouped by period; each item displays period and availability.
- Detail view should support accessible reading and only approved download/print behavior.
- Loading, no statements, source unavailable, and access denied states.

## WF-04 Transfer flow

1. Choose transfer type (NEFT / RTGS / IMPS when enabled).
2. Select/add destination according to bank policy; enter required details.
3. Enter amount and any required scheduling/options.
4. Review destination, amount, transfer type, charges/timing disclosures.
5. Complete required verification and confirm.
6. Show authoritative result, reference, next step; handle pending/unknown without unsafe retry.

Required variants to design: invalid details; limit/policy rejection; service timeout; duplicate submission prevention; pending status; success; failure/reversal; unsupported rail/outside service window.

## WF-05 Utility payment

- Biller discovery/search; biller selection; account/reference fields; bill details validation; amount due and due date where available.
- Review and confirmation; approved authentication; receipt/reference and clear status.
- No biller available, validation error, provider unavailable, bill already paid, duplicate/timeout, and payment status unknown states.

## WF-06 Credit-card details and statements

- Card identity using approved masking; status and approved balance/limit fields.
- Sections or tabs clearly distinguishing current statement, previous statement, and detailed activity.
- Transaction rows with date, description, amount, and any approved status; filters only if in scope.
- Statement unavailable, blocked card, access denied, and processing states.

## WF-07 Card balance payment

- Select eligible card and approved source account.
- Select permitted amount option or enter amount; validate policy-specific boundaries.
- Review amount, card, source, expected timing, and any applicable disclosure.
- Confirm with required verification; show authoritative status/reference.
- Handle payment pending, rejected, duplicate tap, source unavailable, and card not eligible.

## Cross-screen UX requirements to validate

Consistent navigation/back behavior; responsive layouts and supported devices; WCAG/accessibility target to be agreed; keyboard/screen-reader labels; sufficient contrast; clear focus; non-color-only status; localized currency/date formats; secure session timeout; no reliance on color alone; plain language for payment status.
