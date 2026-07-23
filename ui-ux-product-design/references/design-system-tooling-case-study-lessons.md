# Design System and Tooling Case Study Lessons

Use this reference when a UI/UX task involves design systems, theming, tokens, Figma structure, design plugins, agentic design systems, design-to-code, voice/multimodal products, schedule/navigation research, support flows, or internal tools that make product teams faster.

Source creator: [Alex Chiu](https://mchiu.co.uk/). Original pages remain authoritative for project roles and collaborators.

Sources:

- Simplestream design system: https://mchiu.co.uk/case-studies/simplestream-design-system/
- Rayo schedule: https://mchiu.co.uk/case-studies/rayo-schedule/
- Rayo in Alexa: https://mchiu.co.uk/case-studies/rayo-in-alexa/
- Figma plugin Layer Lint: https://mchiu.co.uk/case-studies/figma-plugin-layer-lint/
- Agentic design system: https://mchiu.co.uk/case-studies/agentic-design-system/
- Rayo design system: https://mchiu.co.uk/case-studies/rayo-design-system/
- Figma plugin Rayo thumbnails: https://mchiu.co.uk/case-studies/figma-plugin-rayo-thumbnails/

## Contents

- Core philosophy
- Case 1: Simplestream design system
- Case 2: Rayo schedule
- Case 3: Rayo in Alexa
- Case 4: Layer Lint
- Case 5: Agentic design system
- Case 6: Rayo design system
- Case 7: Rayo thumbnails plugin
- Combined heuristics

## Core philosophy

Use the two screenshots supplied with this update as top-level principles:

- Great UX creates confidence and control: users can predict outcomes, recover from mistakes, and move through a flow without second-guessing.
- Design systems improve speed and consistency only when they protect user experience. Treat them as living foundations, not rigid constraints.

These lessons belong in a reference file rather than the main skill body. The main skill should stay compact; detailed case-study reasoning should load only when the task needs design systems, agentic workflows, tooling, or voice/schedule examples.

## Case 1: Simplestream design system

Source: https://mchiu.co.uk/case-studies/simplestream-design-system/

### Core lesson

A design system should make scale reliable. Simplestream's white-label system reduced brand switching from minutes of fragile plugin work to seconds by restructuring tokens and files around Figma's native library swap behavior.

### Design moves to reuse

- Prefer native platform capabilities over fragile third-party workflow patches when reliability matters.
- Design token naming around the operation the team needs to perform repeatedly.
- Give clients brand flexibility while protecting accessibility-critical rules such as readable typography.
- Treat design-system refactors as product work when they reduce errors, onboarding friction, or maintenance cost.

### Visuals worth inspecting

- Figma Swap Library demo.
- Colour token structure.
- Typography/type-scale treatment.
- Design library swap in action.
- Multi-client platform collage.

### Red flags to catch

- System workflows require anxious waiting, manual checking, or cleanup.
- Token names work visually but fail when libraries, code, or agents need predictable structure.
- Brand flexibility is allowed to undermine readability or accessibility.

## Case 2: Rayo schedule

Source: https://mchiu.co.uk/case-studies/rayo-schedule/

### Core lesson

Research can and should overturn the brief. The product brief asked for station pages, but testing showed listeners needed a schedule-first route to catch-up radio because they think in date and time, not episode taxonomy.

### Design moves to reuse

- Prototype the stakeholder's idea and the suspected alternative, then test behavior instead of arguing in theory.
- Use tree tests, journey mapping, content constraints, and real listener sessions to build evidence.
- Match navigation language to the user's mental model.
- Surface the useful component in existing flows instead of hiding it behind a new destination page.

### Visuals worth inspecting

- Station page epic overview.
- Information architecture explorations and tree test.
- User journey map for core scenarios.
- Radio page prototypes vs schedule page design.
- User testing synthesis affinity map.
- Final schedule mockups.

### Red flags to catch

- A feature is logically complete but users would not navigate to it.
- Product taxonomy uses internal terms where users think by time, task, or situation.
- Research artifacts exist but do not change scope or prioritization.

## Case 3: Rayo in Alexa

Source: https://mchiu.co.uk/case-studies/rayo-in-alexa/

### Core lesson

Invisible flows need visible maps. The Alexa skill had fragmented account-linking paths, silent failures, and scattered support content. Rebuilding journeys in Voiceflow created a shared source of truth and let the team simplify account linking and help.

### Design moves to reuse

- Experience the product as a first-time user before relying on team assumptions.
- Map intents, utterances, synonyms, account states, and failure paths for voice products.
- Consolidate multiple broken paths into one reliable path.
- Align support/help content with the redesigned product flow.
- Add in-situ help where users get stuck instead of sending them away from the task.
- Frame setup or linking around a tangible user benefit.

### Visuals worth inspecting

- Echo Show skill homepage.
- Journey mapping board.
- Interaction model documentation.
- Voiceflow map.
- Account-linking screens.
- Help center support page.
- Continue listening feature.

### Red flags to catch

- Voice interaction only works when users say exact hidden phrases.
- Product and help center describe different realities.
- Account linking, permissions, or authentication paths multiply without a single reliable route.
- Failures are silent or blame another surface.

## Case 4: Layer Lint

Source: https://mchiu.co.uk/case-studies/figma-plugin-layer-lint/

### Core lesson

Layer names are an interface. For agents, design-to-code tools, audits, and engineers, names like `Rectangle 47` force guessing; semantic names like `product-card` transmit intent.

### Design moves to reuse

- Treat cleanup as a product flow: scan, explain why each item is flagged, allow select-all or selective action, then apply.
- Rename by purpose rather than appearance.
- Make AI suggestions reviewable: edit, accept, skip, and avoid destructive bulk changes without review.
- Protect component-instance boundaries so cleanup does not create local overrides.
- Show model choice, cost, retries, and status when an AI tool may take time or fail.

### Visuals worth inspecting

- Cleanup and rename tabs.
- Hidden/empty layer scan result.
- AI-proposed names alongside originals.
- Settings with model selection and API key management.
- Raw vs cleaned layer panel comparison.

### Red flags to catch

- Design files look fine visually but are unreadable to tools.
- AI renaming or cleanup applies changes without user review.
- Plugins modify instance internals and create hidden maintenance debt.
- Tool errors leave users wondering whether the system is stuck.

## Case 5: Agentic design system

Source: https://mchiu.co.uk/case-studies/agentic-design-system/

### Core lesson

An agentic design system is not just documentation for humans; it is instructions for machines. Agents can audit drift, sync tokens, and reason about components only when Figma, code, names, states, and descriptions are structured semantically.

### Design moves to reuse

- Use layered tokens: primitive values, semantic intent, and component-specific aliases.
- Keep Figma variables and code tokens aligned by name and meaning.
- Make component descriptions machine-readable: purpose, props, tokens, states, behavior, and code path.
- Use dark mode as a proof that semantic token architecture works.
- Split canonical files by job: token source of truth vs component source of truth.
- Measure design-system health through gaps, drift, redundancy, missing states, and hardcoded values.

### Visuals worth inspecting

- Three-layer token architecture diagram.
- Storybook light/dark mode validation.
- Component descriptions in Figma.
- Drift audit output comparing code and Figma.
- Organized Figma sections.
- Storybook design tokens page.

### Red flags to catch

- AI is asked to generate from a system that has no semantic structure.
- Tokens exist but do not map cleanly between Figma and code.
- Components are visually documented but lack state, prop, or behavior descriptions.
- Generic agent output is blamed on AI when the design system gave it weak instructions.

## Case 6: Rayo design system

Source: https://mchiu.co.uk/case-studies/rayo-design-system/

### Core lesson

Scalable design systems reduce complexity without reducing flexibility. Rayo's refactor replaced variant explosion with nested components, semantic color variables, responsive foundations, and clearer file architecture.

### Design moves to reuse

- Reduce variants by extracting repeated substructures into nested components.
- Use primitive and semantic color variables to support light/dark modes without manual overrides.
- Treat responsiveness as a system primitive: spacing, radii, breakpoints, and auto-layout rules.
- Organize files around discoverability for new designers.
- Pair documentation with Dev Mode or implementation notes so design intent survives handoff.

### Visuals worth inspecting

- Component optimization before refactor.
- New reusable background/gradient component.
- Component examples across breakpoints.
- Updated system architecture.
- Responsive component structure.

### Red flags to catch

- Variants encode every visual combination instead of exposing reusable parts.
- Manual theme switching creates production risk.
- Designers duplicate components because system architecture is hard to navigate.
- New team members need tribal knowledge to use the system correctly.

## Case 7: Rayo thumbnails plugin

Source: https://mchiu.co.uk/case-studies/figma-plugin-rayo-thumbnails/

### Core lesson

Internal tools should remove repetitive work while preserving user confidence. The Rayo Thumbnails plugin connects directly to live APIs so designers can populate region-specific assets and metadata without stale libraries or manual asset hunting.

### Design moves to reuse

- Bring live data into the design workflow when assets change too often for manual libraries.
- Let users filter by the dimensions that match their work: region, station, content type, show, podcast, episode.
- Keep plugin flows stepwise and obvious: select context, choose content, apply to selected layers.
- Use actionable error guidance when layer names or selections are wrong.
- Iterate internal tools by observing real team behavior.

### Visuals worth inspecting

- Plugin V1 through V5 progression.
- Region/station/content-type picker.
- Podcast and episode interfaces.
- Error guidance overlays.
- Live API-populated thumbnail examples.

### Red flags to catch

- Designers spend hours sourcing assets that already exist in an API.
- Design files go stale because content libraries require manual maintenance.
- Error messages explain failure but not how to fix the selected layer or naming issue.
- Internal tools optimize one local case but fail across regions or markets.

## Combined heuristics

### Design systems

Make the system easier to use than working around it. Reduce duplication, encode semantic intent, document states, and treat user experience as the reason for the system.

### Design tooling

Use tools to remove repetitive work, not judgment. Automate asset fetching, cleanup, renaming, validation, and drift checks while keeping review, intent, and recovery visible.

### Agent-readable design

Assume design files will be read by machines. Names, layers, tokens, states, descriptions, and file architecture are part of the product interface.

### Voice and support flows

Map the invisible. Voice interactions, account linking, support content, and backend states should share one coherent journey model.

### Research-led pivots

Challenge the brief with evidence. When research shows users think in a different structure, change the product direction rather than decorating the original assumption.
