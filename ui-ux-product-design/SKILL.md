---
name: ui-ux-product-design
description: Product UI/UX design, redesign, and review for application screens, dashboards, expert tools, AI-assisted experiences, design systems, editorial/content platforms, Figma/plugin workflows, service/status flows, ecommerce, UGC/reviews, onboarding, financial CRM, 3D configurators, startup MVPs, enterprise healthcare, agile UX delivery, wellbeing/accessibility, sensitive mobile/payment products, search/discovery, recruiting marketplaces, event/booking flows, security/IoT apps, forms, workflows, data visualizations, and product interfaces. Use when improving clarity, usability, visual hierarchy, interaction flow, information architecture, edge cases, states, accessibility, trust, consent, workspace efficiency, design-system scalability, agent-readable design files, or product quality; when reviewing UI screenshots/codebases for UX issues; or when creating product UI that should feel intentional rather than generic.
---

# UI/UX Product Design

## Core posture

Design from the user's job, not from the requested widget. Before polishing a screen, identify what the user is trying to decide, enter, compare, recover from, or complete.

Prefer product clarity over decorative sophistication. A beautiful UI that preserves the wrong mental model is still wrong.

Make users feel in control: they should know where they are, what they can do, what just happened, and what will happen next.

Treat design systems as living foundations, not rulebooks. Use system patterns to increase confidence and consistency, but challenge them when they block the right user experience; feed successful exceptions back into the system.

## Reference routing

Load references only when they match the task. Use one primary reference for the product domain; add one supporting reference when the work crosses systems, AI, research, or sensitive trust patterns. Do not load every reference by default.

When several references seem relevant, choose in this order:

1. **Primary workflow**: the closest user job, market, or product surface.
2. **System constraint**: design system, delivery, data, AI, or platform structure.
3. **Risk layer**: trust, privacy, accessibility, emotional load, safety, or high-stakes recovery.

| Task pattern | Read |
| --- | --- |
| Dashboards, data visualization, input misuse, user-flow simplification, edge-case reduction | `references/michele-du-case-study-lessons.md` |
| Expert workspaces, industrial tools, AI/wearables, health-adjacent products, creative tools, social participation | `references/expert-ai-social-case-study-lessons.md` |
| Design systems, tokens, Figma/plugin tooling, design-to-code, agent-readable files, voice/multimodal flows | `references/design-system-tooling-case-study-lessons.md` |
| Travel/status pages, logistics updates, consumer learning, coaching marketplaces, cultural/nonprofit sites, AI/SaaS landing clarity | `references/service-status-brand-case-study-lessons.md` |
| Ecommerce returns, conversion or abandonment metrics, onboarding activation, clinical/field research, measurable UX impact | `references/research-impact-case-study-lessons.md` |
| Ecommerce discovery, AI shopping summaries, ratings/reviews, reviewer profiles, UGC loops, scalable review templates | `references/commerce-ugc-ai-case-study-lessons.md` |
| Enterprise healthcare, claims/recovery workflows, design-system governance, agile slicing/handoff, AI wellbeing/accessibility | `references/enterprise-systems-delivery-case-study-lessons.md` |
| Sensitive mobile apps, business communications, youth wellbeing, payments, life-admin, trusted contacts, legacy access | `references/sensitive-mobile-product-case-study-lessons.md` |
| Search/discovery, data archives, public portals, recruiting/job marketplaces, resume AI, role dashboards, applicant pipelines | `references/search-job-marketplace-case-study-lessons.md` |
| Publishing, social/community platforms, reader/author UX, typography systems, multi-brand platforms, dense software chrome | `references/editorial-typography-platform-case-study-lessons.md` |
| Startup MVPs, investor prototypes, 3D configurators, financial CRM/mortgages, technical storytelling, AI strategy tools | `references/startup-ai-finance-configurator-case-study-lessons.md` |
| Home cybersecurity, parental controls, IoT monitoring, event/ticketing, seat maps, cinema/streaming, access tools | `references/consumer-security-entertainment-case-study-lessons.md` |

Treat every case-study reference as a reasoning source, not a style kit. Reuse the product move: what problem was reframed, what evidence changed the design, what UI mechanism improved confidence, and what final state proved the work.

## Source use and attribution

When a case study materially shapes a recommendation, add a brief source note naming its creator and linking the original page. Keep the recommendation independently reasoned.

Do not reproduce portfolio screenshots, artwork, logos, or substantial source text. Do not imply that a referenced creator endorses, contributed to, or is affiliated with the resulting work.

## Workflow

### 1. Frame the real problem

State the product job in one sentence:

`User needs to [do/understand/decide] so they can [outcome].`

Then separate:

- **Surface request**: what the user or stakeholder asked for.
- **Actual friction**: what prevents successful use.
- **Success signal**: how the redesign proves it worked.

If the request is "make it nicer," inspect whether the real issue is clarity, hierarchy, missing state, wrong default, poor grouping, terminology, data overload, or a mismatch between user intent and system model.

### 2. Audit before redesigning

For existing screens, audit in this order:

1. **Primary task**: Can a new user tell what to do first within 3 seconds?
2. **Mental model**: Does the UI use concepts users naturally understand?
3. **Hierarchy**: Are the most important actions and readings visually dominant?
4. **Grouping**: Are related controls, data, and actions close together?
5. **Defaults**: Does the default state match the most likely user intent?
6. **Copy**: Is guidance task-specific, short, and placed where action happens?
7. **Feedback**: Are validation, loading, success, empty, and error states explicit?
8. **Data legibility**: Are numbers, labels, trends, and comparisons scannable?
9. **Trust and consent**: Are automated or sensitive actions explained, user-approved, and reversible?
10. **Workspace efficiency**: Does the UI preserve context and reduce repetitive physical/mental work?
11. **System fit**: Does the design system help users and makers move faster without forcing a worse experience?
12. **Machine readability**: If design files feed code or agents, are layers, tokens, states, and components semantically structured?
13. **Edge cases**: Do extremes simplify or break the design?
14. **Accessibility**: Check contrast, keyboard path, focus, labels, target size, and reduced-motion assumptions.

Output findings as user-facing design issues, not taste preferences.

### 3. Choose the right intervention

Use the smallest intervention that changes user behavior:

- **Wrong question**: Reframe the dashboard or screen around the decision users actually need.
- **Wrong default**: Change the default tab, sort, mode, or primary action.
- **Wrong input**: Constrain or transform the input instead of relying on placeholder text.
- **Wrong hierarchy**: Move, group, resize, or de-emphasize content so the primary task is obvious.
- **Wrong visualization**: Replace clever shapes with charts that support comparison and scanning.
- **Wrong flow**: Break competing tasks into steps; separate promotional content from task guidance.
- **Wrong complexity**: Remove modes or interactions that add implementation cost without user value.
- **Wrong automation**: Keep humans in control of AI, body-affecting, or high-stakes decisions; expose why the system recommends or acts.
- **Wrong workspace**: Preserve the primary canvas/context and move secondary controls into collapsible, inspectable, or asynchronous surfaces.
- **Wrong system constraint**: Break or extend the design system pattern when user experience requires it, then document the improved pattern.
- **Wrong file structure**: Rename, organize, or document design layers/tokens/components so humans, engineers, and agents can understand them.

### 4. Design the screen

For new or redesigned UI, produce the usable product surface first. Do not create a marketing landing page unless the user asked for one.

Define:

- **Information architecture**: page regions, navigation, content groups, and progressive disclosure.
- **Primary workflow**: entry point, action path, confirmation, and recovery path.
- **Component choices**: use familiar controls for the job: tabs for peer views, segmented controls for modes, toggles for binary settings, inputs/steppers/sliders for values, menus for bounded option sets, tables for dense comparison, cards for repeated entities.
- **Visual hierarchy**: one dominant job per screen; supporting actions should be visible but quieter.
- **States**: default, hover/focus, loading, empty, invalid, success, warning, destructive, disabled, and overflow.
- **Responsive behavior**: define what stacks, collapses, truncates, or becomes a drawer/sheet on small screens.

### 5. Validate the design

Before finishing, run this check:

- Can the intended user complete the primary task without reading explanatory prose?
- Does every prominent element answer "what is this, why does it matter, what can I do?"
- Are long numbers abbreviated or formatted for scanning while preserving precision where needed?
- Does color encode meaning consistently, with non-color backup when meaning is critical?
- Are the most dangerous mistakes blocked, redirected, or made recoverable?
- Are edge cases handled by a coherent rule rather than one-off patches?
- Does the UI still work with realistic data volume, long labels, missing data, and narrow widths?

## Product design heuristics

### Solve the right problem

When a stakeholder asks for a specific visualization or layout, ask what decision the view must support. If detailed completeness makes the interface harder to use, summarize around the user's outcome and provide drill-down only where useful.

### Use metrics to locate friction and research to explain it

Analytics can show where a journey leaks, but rarely why users lose confidence. Pair funnel/order/support data with interviews, observation, usability testing, benchmark review, and firsthand service walkthroughs before choosing an intervention.

### Visualize for reading, not decoration

Use charts and graphics to improve comparison, trend detection, or prioritization. Avoid ambiguous same-hue palettes, irregular shapes that obscure scale, decorative proportionality, and huge exact numbers that slow scanning.

Use concise numeric formats in overview contexts (`2.8M`, `14.2k`, `+12%`) and expose exact values in tooltips, details, or exports when needed.

### Fix misuse by changing the affordance

If users repeatedly enter the wrong thing, do not assume more helper text will solve it. Consider:

- A prefix/suffix mask that shows what part users should enter.
- Inline normalization or validation with a redirect to the right tool.
- A clearer default tab or entry point.
- Contextual help behind an icon when explanation is useful but not always needed.
- Copy placed beside the control, not in a competing promotional block.

### Let edge cases simplify the model

Use extremes to define a compact rule. If supporting all possible modes creates friction, reduce the mode set to the few perspectives that cover real user needs. Avoid adding horizontal scrolling, nested interactions, or extra views unless the user truly needs that control.

### Preserve flow

Keep task guidance, promotional messaging, destructive warnings, and secondary actions from competing in the same visual layer. When users must make a decision before continuing, make it a step in the flow rather than a dense paragraph near the main task.

### Slice delivery around outcomes

In agile product work, slice design by user value, hypothesis, and buildable increment rather than by static page. Each slice should explain what changes, why it matters, how it behaves, what is already existing, and what evidence or approval moves it forward.

### Design status and service flows around relief

For travel, logistics, service recovery, or any "what is happening now?" product, make the current state, next action, timing, disruption, and recovery path visible before secondary content. Do not bury the answer in forms, modals, weak labels, or visually ambiguous cards.

### Design expert workspaces around context preservation

For scientific, industrial, operational, or IDE-like tools, prioritize the user's working canvas. Collapse navigation, batch repetitive actions, surface status without hover-only discovery, and support asynchronous work so expert users can continue while the system processes.

### Make AI legible, bounded, and consentful

For AI-assisted products, especially health, pregnancy, finance, or other sensitive contexts, explain what data informed the recommendation, what the system will do, and what remains under user control. Never make body-affecting, high-stakes, or identity-sensitive automation feel magical or unavoidable.

### Design context before automation

For AI-assisted product strategy, intake, recommendations, or generation, treat context as part of the UX. Structure inputs, assumptions, expert references, confidence signals, and human QA so the system guides better judgment instead of pretending to be autonomous certainty.

### Design discovery for uncertain intent

When users do not know the exact term, dataset, role, or opportunity they need, design alternate starting points: recommendations, popular searches, categories, breadcrumbs, examples, and guided narrowing. Separate ideal intelligent search from what is technically feasible in the current release.

### Match inventory complexity to user intent

For events, films, streaming, marketplaces, and curated catalogs, the right browsing model depends on why users came: spontaneous discovery, planned booking, specific item lookup, nearby availability, favorite venue, or on-site admission. Use navigation, sorting, filtering, and booking depth to match those intents instead of making one generic feed do everything.

### Model multi-sided workflows by role and shared status

For marketplaces and pipelines, each role needs its own dashboard, permissions, language, and next action, but the shared object should keep one coherent status model. Make handoffs, ownership, completion, documents, feedback, and recovery visible across roles.

### Treat typography as interface structure

Typography is not only styling. Use type to clarify interaction state, hierarchy, reading rhythm, content ownership, density, and brand tone. In dense tools, typography can distinguish labels from actions; in editorial products, it can carry place, pacing, and authorial voice.

### Let platform systems carry distinct voices

For multi-brand, multi-author, or community products, define a shared structural system first, then create controlled areas for expression. The system should improve performance, consistency, and production speed without making every publication, story, or community interaction feel like a reskinned template.

### Design reviews and generated summaries for trust

For ecommerce UGC, do not hide the source material behind summaries, scores, or gamification. Show what is AI-generated, link back to reviews or item details, make contribution impact visible, and collect richer feedback without making the user feel trapped in a long form.

### Make sensitive products calm and structured

For wellbeing, payments, family, legacy, or business-critical communication products, reduce friction without flattening nuance. Use calm hierarchy, predictable steps, visible feedback, permissioned sharing, and clear recovery paths so users can act confidently in emotionally or operationally loaded moments.

### Make invisible risk concrete

For security, privacy, family safety, and network-monitoring products, translate abstract threats into answerable user questions, visible device/activity models, simple controls, and reassuring summaries. Avoid fear as the primary interface pattern; give users understandable state and quick action.

### Lower emotional and social friction

For creative or social products, design for confidence and participation. Let users try privately, iterate without penalty, understand who is involved, and join or share with enough context to feel safe.

### Make brand sites explain the offering

For startups, nonprofits, cultural institutions, and service businesses, visual identity should clarify the promise, not only set a mood. Lead with what the organization offers, who it is for, why it is credible, and what the visitor can do next.

### Build MVPs around proof, not breadth

For early products, investor prototypes, and founder tools, identify the smallest experience that proves the market, workflow, or technical premise. Pair roadmap phases with evidence, cost, risk, and what can ship now; do not design the whole future as if it is the first release.

### Build design systems as product infrastructure

Use design systems to make the right thing easier: reduce variants, use semantic tokens, document states, expose responsive behavior, and align Figma structure with implementation. Optimize for adoption, confidence, and maintainability, not maximum rule count.

### Make design files useful to machines

When design files drive implementation, treat layer names, component descriptions, token names, and file architecture as part of the interface. Semantic structure reduces guessing for design-to-code, QA, accessibility checks, and AI agents.

### Map invisible flows

For voice, multimodal, account linking, support, or complex backend logic, create a visible source of truth before redesigning. Map intents, failure paths, help content, and recovery states so the user experience is coherent across product and support surfaces.

## Response patterns

For a design review, lead with prioritized issues:

`[Severity] Issue - Evidence - Why it matters - Recommended change`

For a redesign proposal, include:

- Problem framing.
- Key screen structure.
- Primary workflow.
- Component/state details.
- Data/edge-case handling.
- Accessibility and responsive notes.

For implementation work, apply the design directly in code, then verify the screen visually at desktop and mobile sizes when possible.
