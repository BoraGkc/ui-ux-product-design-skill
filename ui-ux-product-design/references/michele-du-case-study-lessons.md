# Michele Du Case Study Lessons

Use this reference when a UI/UX task needs product reasoning examples from these case studies:

Source creator: [Michele Du](https://micheledu.com/). Original pages remain authoritative for project roles and collaborators.

- Solve the Right Problem: https://micheledu.com/case-study/solve-right-problem
- Visualize Data: https://micheledu.com/case-study/visualize-data
- Fix Misuse: https://micheledu.com/case-study/fix-misuse
- Edge Case: https://micheledu.com/case-study/edge-case

## Contents

- How to use the case studies
- Case 1: Solve the Right Problem
- Case 2: Visualize Data
- Case 3: Fix Misuse
- Case 4: Edge Case
- Visual selection rule

## How to use the case studies

Use these pages as reasoning references, not as a style kit to copy. Preserve the underlying design moves:

1. Reframe from requested artifact to user decision.
2. Prefer scanability over visual cleverness.
3. Change controls and defaults when users misuse a feature.
4. Use edge cases to reduce, not expand, complexity.

When inspecting visuals, focus on before/after states, rejected explorations, annotated audits, and final design analysis. Skip decorative cover imagery, logos, repeated responsive versions, and raw data screenshots unless the task specifically needs them.

## Case 1: Solve the Right Problem

Source: https://micheledu.com/case-study/solve-right-problem

### Core lesson

Do not refine a visualization until the underlying user question is validated. The original dashboard attempted to show lifecycle completeness, but the more useful need was understanding risk movement and mitigation progress.

### Design moves to reuse

- Translate a broad visualization request into user questions.
- Compare micro-level clarity against macro-level confusion.
- Replace a static disconnected view with a dashboard that connects sources, stages, and outcomes.
- Keep the most relevant monitoring and progress information in one viewport when the user is comparing operational state.

### Visuals worth inspecting

- Original three-stage lifecycle funnel/dashboard.
- Bubble graph exploration.
- Bar/funnel exploration with too much same-hue color and crowding.
- Annotated dashboard audit.
- Transition diagrams that reveal why granular lifecycle flow becomes confusing at scale.
- Final dashboard and design analysis.

### Red flags to catch in future designs

- The screen shows the system model but not the user's decision.
- The visualization is technically complete but operationally hard to act on.
- The chart preserves a familiar metaphor after the metaphor stops serving the task.

## Case 2: Visualize Data

Source: https://micheledu.com/case-study/visualize-data

### Core lesson

Data visualization in reports should make the message readable. Perfect proportional scaling and impressive graphic forms can be less useful than simpler encodings that support quick comparison.

### Design moves to reuse

- Reduce ambiguous color families into distinct roles.
- Replace irregular shapes, bubbles, or arrows with bars when comparison matters.
- Abbreviate large values in overview contexts.
- Add trend indicators when direction is as important as the raw number.
- Keep report pages scannable for both technical and non-technical readers.

### Visuals worth inspecting

- Bubble-size/proportionality explanation.
- Color simplification from many purple shades into fewer distinct styles.
- Before/after report covers.
- Reworked horizontal bar charts.
- Final design showcase pages showing readable numbers and trends.

### Red flags to catch in future designs

- Too many shades of one color encode different meanings.
- Users must compare area, trapezoid width, or decorative forms instead of aligned lengths.
- Exact numbers dominate where abbreviated values would be more legible.
- Static report visuals look impressive but slow comprehension.

## Case 3: Fix Misuse

Source: https://micheledu.com/case-study/fix-misuse

### Core lesson

Repeated misuse is often a control-design failure, not a user-reading failure. If users paste a URL where a domain is required, helper text alone may not work because the user's mental model is different.

### Design moves to reuse

- Identify misuse patterns from behavior, not only stated feedback.
- Separate URL scanning from domain monitoring when users confuse them.
- Use a pre-fill mask or segmented input to show which part belongs in the field.
- Provide inline correction and a route to the right tool when the entered data belongs elsewhere.
- Move promotional messaging away from the main task flow.
- Set the default tool to match the most common first-time user intent.

### Visuals worth inspecting

- Original CheckPhish domain-monitoring screen.
- URL vs domain explainer sketch.
- Design audit showing competing instructions and promotion.
- Inline error/correction state.
- Pre-fill mask input solution.
- Flow improvement screens that separate export reminder, upsell, and monitoring.
- Web version with URL scanner as the default entry point.

### Red flags to catch in future designs

- Placeholder text tries to teach a concept users do not understand.
- Promotional copy competes with task instructions.
- The default tab is optimized for the product's internal category, not the user's intent.
- The UI accepts a common wrong input and only complains after submission.

## Case 4: Edge Case

Source: https://micheledu.com/case-study/edge-case

### Core lesson

Edge cases can be used as a design tool. By designing for the extremes, a product can reduce the number of modes and create a simpler rule that works for most users.

### Design moves to reuse

- Identify the maximum and minimum realistic ranges before adding modes.
- Remove modes that exist only because a prototype made them possible.
- Prefer two meaningful perspectives over many granular controls when users need orientation, not scheduling power.
- Expand days or columns with content and compress empty space.
- Indicate actions outside the current view instead of requiring awkward horizontal scrolling.

### Visuals worth inspecting

- Timeline that cannot handle clustered or widely spaced actions.
- Early multi-mode idea with half-year, month, bi-week, and week views.
- Simplified 6-month and 1-month mode structure.
- Dynamic-width day treatment for crowded actions.
- Final timeline overview and outside-view indicators.

### Red flags to catch in future designs

- Edge cases add more controls instead of clarifying the core rule.
- The design combines horizontal and vertical scrolling in a dense table.
- Users get project-management affordances when they only need progress transparency.
- Empty time periods consume as much attention as days with real events.

## Visual selection rule

When building a reference deck, skill asset, or design critique from these pages, capture only visuals that answer one of these questions:

- What was wrong with the first solution?
- What alternatives were explored and rejected?
- What user need reframed the design?
- What concrete UI mechanism fixed the issue?
- What final screen proves the new hierarchy or flow?

Avoid visuals that are purely decorative, repeated, or only aesthetic unless the task is specifically about portfolio storytelling.
