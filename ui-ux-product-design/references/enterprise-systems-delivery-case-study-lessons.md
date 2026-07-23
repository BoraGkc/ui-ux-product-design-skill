# Enterprise Systems and Delivery Case Study Lessons

Use this reference when a UI/UX task involves enterprise healthcare platforms, insurance claims or recovery workflows, complex internal tools, design-system governance, pattern libraries, agile UX delivery, design slicing and handoff, AI-assisted product creation, AI wellbeing products, or AI accessibility strategy.

Source creator: [Nate Bauer](https://nabauer.com/). Original pages remain authoritative for project roles and collaborators.

Sources:

- Centene recovery platform: https://nabauer.com/work/centene-recovery-platform
- Designing systems at scale: https://nabauer.com/work/designing-systems-at-scale
- Daily Noodle: https://nabauer.com/work/daily-noodle
- AI will revolutionize accessibility: https://nabauer.com/articles/ai-will-revolutionize-accessibility
- How UX fits in an agile framework: https://nabauer.com/articles/how-ux-fits-in-an-agile-framework
- Why build design systems: https://nabauer.com/articles/why-build-design-systems
- Slicing: https://nabauer.com/articles/slicing

## Contents

- How to use these case studies
- Case 1: Centene recovery platform
- Case 2: K-T design system
- Case 3: Daily Noodle
- Article lessons: AI accessibility, agile UX, design systems, slicing
- Combined heuristics

## How to use these case studies

Use these as references for product operating model, enterprise complexity, and delivery structure. The strongest shared pattern is that product quality comes from aligning the team, reducing ambiguity, and making each increment understandable to users, stakeholders, designers, and developers.

Inspect visuals that show:

- Product canvas artifacts, team-role diagrams, dual-track agile cadence, and hypothesis prioritization.
- Claims dashboard, claim detail, audit log, saved filter setups, status pills, batch actions, and modal behavior.
- K-T atomic architecture, token/atom/molecule/organism model, naming conventions, governance model, maturity graph, and pattern library examples.
- Daily Noodle mood heatmap, time-capsule answers, observation cards, privacy/data architecture, mobile reflection and community surfaces.
- Slicing diagrams with numbered annotations, color-coded status, slice descriptions, approval states, and page naming.

Skip portfolio cover styling unless the task is specifically about case-study presentation.

## Case 1: Centene recovery platform

Source: https://nabauer.com/work/centene-recovery-platform

### Core lesson

Enterprise healthcare tools need alignment before interface polish. The Centene recovery platform started with a broken claims recovery process, then used product canvas alignment, dual-track agile, hypothesis prioritization, and design slices to evolve across many tested iterations.

### Design moves to reuse

- Start complex enterprise work with a shared product canvas: problem, business goals, users, user needs, questions, and success metrics.
- Make strategic focus explicit. Choose the narrow outcome that can create value quickly instead of trying to solve the entire system at once.
- Use hypothesis prioritization to connect user needs, proposed features, value, effort, and expected outcomes.
- Prefer a proven design system when constraints include legal, maintenance, tech stack, and heavy data manipulation.
- Keep high-volume analyst work centered on tables, filters, sorting, batch actions, status, history, comments, deadlines, and saved setups.
- Preserve context for complex review work: use modals, audit logs, and detail views without making analysts lose their place in the queue.
- Track team health and delivery momentum in addition to user outcomes.

### Visuals worth inspecting

- Product canvas problem, goals, team, and user-needs boards.
- Dual-track agile and waterfall/agile timeline.
- Hypothesis prioritization board.
- Full design slice documentation.
- Analyst claims dashboard, claim detail page, audit log, and saved filters.
- Status pills, batch actions, confirmation modals, date picker, and processing modal.

### Red flags to catch

- Enterprise teams jump into screens before agreeing on the problem, users, success metrics, and current unknowns.
- A platform replaces a legacy tool but preserves the same manual prioritization, spreadsheets, or email handoffs.
- Users can act on a record but cannot see its history, current state, deadline, or reason for being in that state.
- Stakeholders cannot tell what has shipped, what is next, or what hypothesis each increment is testing.

## Case 2: K-T design system

Source: https://nabauer.com/work/designing-systems-at-scale

### Core lesson

Enterprise design systems are alignment systems before they are component libraries. K-T responded to fragmented embedded teams by defining constraints, foundations, naming, governance, maturity, and a pattern layer above components.

### Design moves to reuse

- Use a design-system framework as a starting point, then adapt it to the organization's culture, constraints, tech stack, legal needs, accessibility expectations, and governance model.
- Audit real products before declaring core components; promote only repeated cross-product needs into the system.
- Separate core system primitives from one-off templates and product-specific patterns.
- Add tokens below atomic design so color, typography, spacing, shape, motion, grid, theming, and iconography scale predictably.
- Define naming conventions that work for both design and development, such as component, variant, action, size, type, and state.
- Document what each component is, when to use it, its visual examples, states, properties, and variants.
- Create a governance model so the system can evolve without depending on tribal knowledge.
- Measure design-system maturity and stay at the lowest maturity level that does not block progress.

### Visuals worth inspecting

- Hybrid product-team structure and fragmentation problem.
- Federated-to-centralized system comparison.
- Design System in 90 Days adaptation and constraints list.
- Atomic model with tokens.
- Naming convention examples and definitions.
- 31 core components, documentation pages, governance model, pattern structure, maturity graph, and pattern examples.

### Red flags to catch

- Teams call a component library a design system before documenting purpose, usage, governance, and contribution rules.
- Designers solve the same problem in parallel because embedded team autonomy lacks a shared system.
- Product-specific templates enter the core design system too early.
- The system grows in maturity, complexity, or maintenance cost before the organization needs it.

## Case 3: Daily Noodle

Source: https://nabauer.com/work/daily-noodle

### Core lesson

AI wellbeing products must make insight feel earned, private, and humane. Daily Noodle uses one daily question, instant save, time-capsule answers, mood family compression, and AI reflection to reduce journaling friction while building long-term self-understanding.

### Design moves to reuse

- Solve habit retention by changing product shape: remove the blank page, make the loop tiny, and let payoff compound over time.
- Use AI as an execution layer, but keep human judgment over direction, cuts, privacy, emotional tone, and quality.
- Compress emotional data for readability. Mood categories should scan quickly and carry meaning.
- Never make the user wait for reflection; use instant save, background classification, and progressive insight.
- Let users experience value before signup when possible, then preserve the unsaved entry through authentication.
- Make private the default and sharing explicit per entry.
- Keep personal AI grounded in the user's own words, limited in volume, and tied to concrete suggestions.
- Treat heavy emotional patterns responsibly by pointing toward real help rather than trapping the user in the app.
- Validate honestly: distinguish self-use, early signal, hypotheses, retention metrics, and future tests.

### Visuals worth inspecting

- One-question product loop diagram.
- Mood compression and 52-week heatmap.
- Today screen with past answers to the same annual question.
- Privacy/data architecture.
- AI pattern-analysis flow and observation cards.
- Reflect page, mobile reflect page, and optional community feed.

### Red flags to catch

- AI mental wellbeing output sounds generic, diagnostic, or magical rather than grounded in user writing.
- Journaling asks for too much setup before the first value moment.
- Community or sharing defaults pressure users into performing private reflection.
- Sensitive writing or API keys travel through the browser unnecessarily.

## Article Lessons

### AI accessibility

Source: https://nabauer.com/articles/ai-will-revolutionize-accessibility

AI may reduce accessibility friction by acting as an adaptive layer over imperfect products, but that is not permission to skip accessible design. Use AI to reduce learning curves, translate intent, operate existing interfaces, and augment assistive technology while still designing products to work with accessibility standards, assistive tools, and legal expectations.

Watch for teams using AI accessibility as an excuse to delay semantic structure, keyboard support, labels, contrast, captions, or inclusive testing.

### Agile UX

Source: https://nabauer.com/articles/how-ux-fits-in-an-agile-framework

Agile UX creates value earlier by focusing discovery, design, build, and testing on the highest-value slice first. Waterfall tries to get the full product right on the first try; agile tries to get the product right eventually through smaller releases and feedback.

Use agile when software can ship a useful partial experience. Avoid slicing so thin that no user value or learning remains.

### Design-system timing

Source: https://nabauer.com/articles/why-build-design-systems

Do not build a design system before the component library is creating friction. Start with local components, evolve into a library as screens multiply, then become a system when purpose, usage rules, shared patterns, and team scale require it.

Design systems are commitments. Build only the system the current product and team need, then let it mature as real duplication and inconsistency appear.

### Slicing

Source: https://nabauer.com/articles/slicing

Slicing turns design delivery into a single agile artifact for stakeholders, product, design, and development. A slice should show the design, describe functionality, number annotations, identify new/existing/review/remove changes, include a short objective, and communicate approval status.

Useful slice mechanics:

- Number annotations so documentation points to exact UI regions.
- Use color or status labels for new, existing, under-review, and removed elements.
- Keep previous context where it helps developers understand what changed.
- Put each slice on a numbered page so design and development can work at different stages.
- Add approval state to page names or slice headers.
- Use multiple slices to communicate product momentum and next problems being addressed.

## Combined heuristics

### Enterprise platforms

Design the operating model before the screen. Align roles, goals, users, hypotheses, cadence, and success metrics so the UI solves a known system problem instead of decorating process ambiguity.

### Healthcare and claims work

Design for evidence, history, status, deadline, and handoff. Analysts need to know what happened, why it is in this state, who touched it, what can be done next, and where the work goes after action.

### Design systems

Scale from need, not ambition. Components solve repetition; design systems solve shared decision-making; pattern libraries solve recurring domain structures above components.

### Agile delivery

Value should appear before the whole product is done. Slice around the highest-impact user outcome, test it, learn, and let future slices adapt.

### AI-assisted product creation

Execution getting cheaper makes product judgment more important. Use AI to accelerate exploration and implementation, but keep human responsibility over product shape, privacy, emotional tone, ethical boundaries, and when output is wrong.

### Accessibility

AI can augment access, but accessible foundations still matter. Treat semantic structure, standards, assistive-technology compatibility, and inclusive design as the base layer; use AI to reduce remaining barriers.
