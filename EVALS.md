# UI/UX Product Design Evaluations

Run these prompts in fresh contexts against the packaged skill before release. Judge the required signals, not exact wording. Do not provide the expected signals to the evaluating agent.

## Release status

| Release | Date | Result |
| --- | --- | --- |
| v1.2.0 | 2026-07-23 | 2/2 new cases passed; v1.1.1 suite unchanged |
| v1.1.1 | 2026-07-23 | 2/2 targeted checks passed; v1.1.0 suite unchanged |
| v1.1.0 | 2026-07-23 | 6/6 passed |

Each prompt was run in a fresh context. Cases 5 and 6 used disposable local fixtures outside the repository so implementation and browser behavior could be exercised without shipping test scaffolding.

Cases 9 and 10 were also run in fresh contexts without their expected signals. Case 9 used a disposable local fixture; its result was checked at `1440×900` and `390×844`, including initial requests, selected-provider activation, keyboard membership intent, the accessibility tree, overflow, console output, and failure-recovery code. Case 10 used only the supplied production evidence.

| Case | Result | Release observation |
| --- | --- | --- |
| Operations dashboard review | Pass | Prioritized escalation and undefined states; credited Michele Du. |
| Ecommerce AI review-summary redesign | Pass | Covered provenance, conflicting evidence, recovery, mobile, and Nicole Roberts attribution. |
| Sensitive mobile payment flow | Pass | Covered roles, consent, duplicate recovery, emotional safety, and Jacob Dilley attribution. |
| Search and recruiting marketplace | Pass | Supported uncertain intent, role workspaces, shared status, permissions, and relevant creator credit. |
| Existing application implementation | Pass | Reused the fixture system, implemented complete states, built successfully, and verified both target sizes. |
| Validation-only browser review | Pass | Made no edits and separated observed passes, failures, and unavailable states without redesigning. |
| Standalone logo request | Pass | Routed to image generation without loading the product UI/UX skill. |
| Decorative poster request | Pass | Routed to image generation without loading the product UI/UX skill. |
| Media-heavy homepage implementation | Pass | Deferred media and membership code until intent, preserved fallbacks and recovery, and passed responsive browser checks. |
| Production Lighthouse triage | Pass | Separated application, edge, lab, field, and score-only evidence without proposing interface changes. |

## 1. Operations dashboard review

**Prompt**

> Review an operations dashboard with six equal KPI cards, a 25-slice same-hue pie chart, an incident table, and an Escalate action hidden in each row menu. Loading, empty, error, and partial-data states are unspecified. The user's main job is deciding which incidents to escalate.

**Expected signals**

- Select `review` mode and do not edit or implement.
- Frame escalation as the primary user decision.
- Prioritize the hidden action and undefined operational states.
- Replace or remove the unreadable chart rather than restyle it.
- Route primarily to Michele Du and include a source note if those lessons materially shape the response.

## 2. Ecommerce AI review-summary redesign

**Prompt**

> Redesign an ecommerce AI review-summary panel. Show what informed the summary, link to source reviews, handle missing or conflicting reviews, and work on mobile.

**Expected signals**

- Select `redesign` mode and do not write code.
- Preserve access to original reviews and label generated content.
- Cover provenance, low evidence, disagreement, loading, unavailable, and mobile states.
- Include trust, accessibility, and recovery/reporting behavior.
- Route to Nicole Roberts' commerce/UGC reference and credit it when materially used.

## 3. Sensitive mobile payment flow

**Prompt**

> Redesign a mobile flow that lets a family member request and collect funeral-service payments from trusted contacts. Users may be grieving, permissions differ by role, and failed or duplicated payments must be recoverable.

**Expected signals**

- Select `redesign` mode.
- Frame the job calmly without flattening the emotional context.
- Define roles, consent, confirmation, duplicate prevention, failure, retry, reconciliation, and trusted-access states.
- Address mobile target sizes, focus, non-color status, and plain-language copy.
- Route to Jacob Dilley's sensitive-mobile reference and credit it when materially used.

## 4. Search and recruiting marketplace

**Prompt**

> Redesign a recruiting marketplace where applicants do not know the right job title to search, employers manage pipelines, and consultancies collaborate across several clients.

**Expected signals**

- Select `redesign` mode.
- Support uncertain search with categories, examples, recommendations, and guided narrowing.
- Separate role dashboards while preserving a shared applicant/job status model.
- Cover permissions, ownership, handoffs, empty results, saved searches, and recovery.
- Route to the search/job-marketplace reference and credit the relevant creator when materially used.

## 5. Existing application implementation

**Prompt**

> Implement a clearer account settings screen in an existing React application. Reuse its current design system and components. The screen must support profile editing, notification preferences, password changes, destructive account deletion, and mobile layouts.

**Expected signals**

- Select `implement` mode and inspect the repository before editing.
- Reuse existing tokens, components, utilities, and dependencies.
- Load visual craft only for unresolved choices and avoid inventing a replacement visual system.
- Implement validation, success, disabled, destructive confirmation, and error states.
- Run existing checks and verify at `1440×900` and `390×844`, reporting anything not verified.

## 6. Validation-only browser review

**Prompt**

> Validate the current checkout UI at desktop and mobile sizes. Do not redesign or modify it. Report accessibility, responsive, state, overflow, and console findings.

**Expected signals**

- Select `validate` mode and make no edits.
- Separate pass, fail, and blocked results.
- Inspect at `1440×900` and `390×844`.
- Check keyboard order, focus, labels, target sizes, long content, horizontal overflow, relevant states, reduced motion, and console errors.
- Never claim a check passed if the environment or state was unavailable.

## 7. Standalone logo request

**Prompt**

> Design a standalone logo and color palette for a neighborhood coffee shop. There is no application, website, or user workflow.

**Expected signals**

- Do not trigger `$ui-ux-product-design`.
- Do not force product-job framing, workflow states, or case-study routing onto the request.
- Route to a branding or image-design capability when one is available.

## 8. Decorative poster request

**Prompt**

> Make this concert poster feel more experimental with custom illustration and expressive typography. It is a static print piece with no interaction.

**Expected signals**

- Do not trigger `$ui-ux-product-design`.
- Do not load product UI references or apply the review/redesign/implement/validate workflow.
- Route to an illustration, image, or graphic-design capability when one is available.

## 9. Media-heavy homepage implementation

**Prompt**

> Implement and validate a media-heavy responsive homepage in an existing web application. It has one lead image, secondary story cards, YouTube and Spotify embeds, and membership controls. Preserve no-JavaScript access, keyboard use, loading and provider-failure recovery, and the existing design system.

**Expected signals**

- Select `implement`, inspect the repository, and load the web delivery reference as the supporting reference.
- Keep static content unhydrated; hydrate only required interaction and defer noncritical controls.
- Make only the lead image eager and high priority; use responsive modern images, lazy secondary media, correct dimensions, and reserved embed space.
- Replace immediate media players with accessible link facades that load only the activated provider.
- Load membership code on intent while preserving disabled, loading, success, failure, retry, and keyboard states.
- Run project checks and inspect desktop and mobile rendering, the keyboard path, initial network requests, accessibility tree, console, and relevant failure states.

## 10. Production Lighthouse triage

**Prompt**

> Validate a deployed website from this Lighthouse evidence: a deprecated API comes from a CDN-injected script; an unknown managed directive appears only in the delivered `robots.txt`; a forced-reflow diagnostic names no attributable function and estimates no savings; and a responsive image selected for a high-DPR display is reported as oversized. Diagnose the findings without changing the interface.

**Expected signals**

- Select `validate`, make no edits, and separate passes, failures, and blocked checks.
- Compare repository output, preview output, the final custom domain, response headers, network requests, and a performance trace.
- Attribute application and edge behavior separately and recommend an edge-layer correction for edge-generated failures.
- Retain security behavior and correct high-DPR image delivery instead of chasing score-only findings.
- Treat unattributed zero-savings diagnostics as unproven unless a repeat trace or user impact supplies evidence.
- Distinguish Lighthouse lab simulation from CrUX or RUM field data and state what could not be verified.
