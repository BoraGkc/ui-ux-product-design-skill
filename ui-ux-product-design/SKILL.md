---
name: ui-ux-product-design
description: Product UI/UX reasoning, redesign, implementation, and validation for application screens, dashboards, workflows, expert tools, AI-assisted and trust-sensitive experiences, and task-oriented product or service websites. Use for user-job framing, information architecture, interaction flow, hierarchy, states, accessibility, responsive behavior, design-system fit, visual craft, and implementation review. Do not use for standalone logos, posters, illustrations, or decorative styling without a user workflow.
---

# UI/UX Product Design

## Core posture

Design from the user's job, not from the requested widget. Identify what the user needs to decide, enter, compare, recover from, or complete before polishing the screen.

Prefer product clarity over decorative sophistication. Make users understand where they are, what they can do, what happened, and what happens next.

Reuse the existing design system, components, and product language before introducing new patterns. Break a system pattern only when it blocks the right experience, then document the improved pattern.

## Choose the operating mode

Infer one mode from the request. Do not expose these as slash commands.

- **Review**: Diagnose without editing. Return prioritized issues with evidence, impact, and the smallest effective change.
- **Redesign**: Propose information architecture, workflow, components, states, responsive behavior, and accessibility. Do not write code unless the user asks.
- **Implement**: Inspect the real code and existing system, reuse what is present, make the smallest complete change, and verify the runnable interface.
- **Validate**: Preserve the current design. Run relevant checks and report pass, fail, and blocked results without redesigning or editing unless explicitly requested.

Respect the authorization implied by the request. A review or validation request does not authorize implementation.

## Reference routing

Load only the references needed for the task. Use one primary domain reference and at most one supporting reference for a system constraint or risk layer.

Read `references/visual-craft.md` only for new UI, restyling, or implementation where the visual direction is open. Skip it when an established design system already resolves the visual decisions or when the task is validation-only.

Choose domain references in this order:

1. Closest user job or product surface.
2. Relevant system constraint: design system, delivery, data, AI, or platform.
3. Relevant risk: trust, privacy, accessibility, emotional load, safety, or recovery.

| Task pattern | Read |
| --- | --- |
| Dashboards, data visualization, input misuse, flow simplification, edge cases | `references/michele-du-case-study-lessons.md` |
| Expert workspaces, industrial tools, AI/wearables, health-adjacent products, creative or social tools | `references/expert-ai-social-case-study-lessons.md` |
| Design systems, tokens, Figma/plugin tooling, design-to-code, agent-readable files, voice flows | `references/design-system-tooling-case-study-lessons.md` |
| Travel/status, logistics, learning, coaching, cultural/nonprofit, product or service websites | `references/service-status-brand-case-study-lessons.md` |
| Ecommerce returns, onboarding activation, clinical/field research, measurable UX impact | `references/research-impact-case-study-lessons.md` |
| Ecommerce discovery, AI summaries, ratings/reviews, reviewer profiles, UGC | `references/commerce-ugc-ai-case-study-lessons.md` |
| Enterprise healthcare, claims/recovery, governance, agile slicing, AI accessibility | `references/enterprise-systems-delivery-case-study-lessons.md` |
| Sensitive mobile, communications, wellbeing, payments, life admin, trusted access | `references/sensitive-mobile-product-case-study-lessons.md` |
| Search/discovery, data archives, public portals, recruiting, role dashboards, pipelines | `references/search-job-marketplace-case-study-lessons.md` |
| Publishing, community platforms, typography, multi-brand platforms, dense software chrome | `references/editorial-typography-platform-case-study-lessons.md` |
| Startup MVPs, prototypes, 3D configurators, financial CRM, AI strategy tools | `references/startup-ai-finance-configurator-case-study-lessons.md` |
| Home security, parental controls, IoT, events, ticketing, cinema/streaming, access tools | `references/consumer-security-entertainment-case-study-lessons.md` |

Treat case studies as reasoning sources, not style kits. Reuse the product move: what problem was reframed, what evidence changed the design, and what mechanism improved confidence.

## Source use and attribution

When a case study materially shapes a recommendation, add a brief source note naming its creator and linking the original page. Keep the recommendation independently reasoned.

Do not reproduce portfolio screenshots, artwork, logos, or substantial source text. Do not imply endorsement, contribution, or affiliation.

## Workflow

### 1. Frame the real problem

State:

`User needs to [do/understand/decide] so they can [outcome].`

Then identify:

- **Surface request**: what was asked for.
- **Actual friction**: what prevents successful use.
- **Success signal**: what observable outcome proves improvement.

If the request is vague, inspect for unclear hierarchy, missing states, wrong defaults, poor grouping, terminology, overload, or a mismatch between user intent and the system model.

### 2. Audit before changing

For an existing interface, inspect in this order:

1. Primary task and first action.
2. User mental model and terminology.
3. Hierarchy and grouping.
4. Defaults and progressive disclosure.
5. Copy at the point of action.
6. Loading, empty, invalid, error, success, disabled, destructive, and overflow states.
7. Data scanability and comparison.
8. Trust, consent, explanation, and reversibility.
9. Context preservation and repetitive work.
10. Existing design-system fit.
11. Realistic data, long labels, missing data, and narrow widths.
12. Contrast, keyboard path, focus, labels, target size, and reduced motion.

Describe user-facing problems rather than taste preferences.

### 3. Choose the smallest effective intervention

Prefer changing the decision, default, input, hierarchy, visualization, grouping, or flow before adding new UI.

- Constrain a repeatedly misused input instead of adding more helper text.
- Replace decorative or ambiguous charts with scannable comparisons.
- Separate competing tasks into steps.
- Keep high-stakes and automated actions explained, permissioned, and recoverable.
- Preserve the primary canvas in expert tools.
- Remove modes and interactions that add implementation cost without user value.

### 4. Design or implement the product surface

Define the usable interface before secondary presentation:

- Information architecture and page regions.
- Primary action path, confirmation, and recovery.
- Familiar controls that match the job.
- One dominant task per screen.
- Required states and realistic content.
- Responsive rules for stacking, collapsing, truncation, drawers, or sheets.

In **implement** mode:

1. Trace the current flow and inspect every affected component.
2. Reuse existing tokens, components, utilities, and dependencies.
3. Load `references/visual-craft.md` only when visual choices remain open.
4. Change the fewest files that produce a complete result.
5. Preserve accessibility and error handling.
6. Run the project's relevant checks.
7. Verify the interface before reporting completion.

### 5. Verify implementation

When a runnable interface exists, verification is required:

- Inspect at `1440×900` and `390×844`.
- Exercise the primary path with keyboard input.
- Check focus visibility, long labels, realistic data, overflow, and horizontal scrolling.
- Check every relevant loading, empty, invalid, error, success, disabled, destructive, and partial-data state.
- Check reduced-motion behavior and browser console errors.
- Capture before and after screenshots for an existing-screen redesign.

Fix issues within the requested scope and repeat the affected checks. If the interface cannot run or browser access is unavailable, state exactly what was not verified and why. Never imply a visual check passed when it was not run.

## Output contracts

For a **review**, use:

`[P0–P3] Issue — Evidence — Why it matters — Recommended change`

For a **redesign**, include problem framing, screen structure, primary workflow, components and states, responsive behavior, accessibility, and edge cases.

For **implementation**, lead with the completed outcome, then report the checks and visual sizes verified.

For **validation**, separate results into pass, fail, and blocked. Do not include redesign suggestions unless the user asks for them.
