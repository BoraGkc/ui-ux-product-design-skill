# Visual Craft

Read this only when creating new UI, restyling an interface, or implementing a screen whose visual direction is not already resolved by an existing design system.

## Start with the system

Inspect the product before inventing a visual language:

- Reuse established tokens, typography, components, icons, breakpoints, and motion.
- Preserve recognizable product patterns unless they cause a documented usability problem.
- Do not add a font, icon library, animation package, or component dependency when the existing stack can produce the result.
- Treat a design-system exception as a product decision, not decoration.

## Define a compact direction

Before implementation, settle six decisions:

1. **Audience and job**: who uses the interface and what must they accomplish?
2. **Visual character**: choose two or three brief-specific qualities such as calm, precise, editorial, utilitarian, warm, or technical.
3. **Color**: define four to six semantic roles—canvas, surface, text, muted text, action, and status—not a collection of fashionable swatches.
4. **Typography**: define two or three roles—display, body, and utility/data when needed—with a clear scale and deliberate weight.
5. **Layout rhythm**: use a consistent spacing base, readable measure, alignment logic, and density suited to the job.
6. **Signature**: choose one memorable element rooted in the product's subject or workflow. Keep the rest disciplined.

Use real content and realistic data. A distinctive interface comes from specific product meaning, not arbitrary visual novelty.

## Make hierarchy do work

- Give the primary job the strongest position, contrast, and available space.
- Group controls with the content they affect.
- Use typography, spacing, dividers, and alignment to encode structure.
- Use cards only for genuinely independent or repeated entities; do not wrap every section in a rounded container.
- Keep secondary actions available but visually quieter.
- Let dense expert interfaces stay dense when density improves scanning and context.

## Avoid generic output

Reject a choice when it could be pasted into any unrelated product without changing:

- Purple-to-blue gradients used as default personality.
- Glass effects without a spatial or interaction reason.
- Repeated icon-heading-copy card grids.
- Decorative charts, sparklines, or oversized metrics that do not support a decision.
- Emoji used as interface icons.
- Arbitrary border radii, shadows, colored side borders, or gradient text.
- Default dark “tech” themes, generic cream editorial themes, or fashionable type pairings unrelated to the subject.
- Multiple competing animations or visual focal points.

Do not avoid a pattern merely because it is popular. Use it when the product meaning and user job justify it.

## Use color and type deliberately

- Preserve contrast for normal text, large text, controls, focus indicators, and status communication.
- Pair color with text, icons, shape, or position when meaning is critical.
- Keep body text readable at narrow widths and zoomed layouts.
- Format numbers for scanning while retaining exact values in details, tooltips, or exports.
- Use labels and copy that describe what users control, not system implementation.

## Use motion with restraint

Choose at most one signature motion pattern and a small set of functional transitions:

- Use motion to explain continuity, hierarchy, progress, or cause and effect.
- Keep feedback immediate and transitions short enough not to delay work.
- Avoid bounce, scattered entrance effects, or motion that exists only to look advanced.
- Respect `prefers-reduced-motion` and ensure the task remains understandable without animation.

## Check responsive behavior

Do not shrink a desktop layout and call it responsive:

- Preserve the primary job and action on small screens.
- Stack by task priority, not DOM convenience.
- Convert dense tables to cards only when cards preserve comparison; otherwise use deliberate responsive columns or a focused detail view.
- Avoid nested scrolling, hover-only information, clipped labels, and horizontal overflow.
- Keep interactive targets usable and focus order logical.

## Critique before finishing

Ask:

- Does the direction belong to this product and audience?
- Is one element memorable while the rest stays coherent?
- Does every decorative choice carry information or reinforce the intended character?
- Does the existing design system remain recognizable?
- Would removing one effect, container, color, or animation improve the result?

Revise any choice that reads as an unexamined AI default.
