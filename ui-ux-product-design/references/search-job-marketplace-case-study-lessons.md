# Search, Job Marketplace, and Public Portal Case Study Lessons

Read this when the design task involves search/discovery, data archives, public service portals, recruiting workflows, applicant pipelines, resume builders, AI writing/review assistance, multi-role marketplaces, or audience-specific landing pages.

Source creators: [Ramachandran Swamy](https://whyramachandran.design/) and [Lawrence Zheng](https://www.lawrencezheng.com/). Original pages remain authoritative for project roles and collaborators.

Sources reviewed:

- Ramachandran, Workruit / Talent Linker case study: https://whyramachandran.design/Case-study-1
- Ramachandran, AI-enhanced resume builder case study: https://whyramachandran.design/Case-study-2
- Ramachandran, DEET website redesign case study: https://whyramachandran.design/Case-study-3
- Lawrence Zheng, ICPSR search redesign case study: https://www.lawrencezheng.com/icpsr

## Contents

- Transferable Lessons
- Visuals Worth Inspecting
- Apply This In Practice

## Transferable Lessons

### Design multi-role marketplaces as linked but separate workspaces

Recruiting platforms serve employers, consultancies, applicants, HR managers, collaborators, and sometimes public-sector partners. Do not force every role into one generic dashboard.

Useful pattern:

- Give each role a dedicated home surface with its own primary task.
- Keep shared entities consistent: applicant, job, interview, offer, document, feedback, profile, collaborator.
- Show role-specific next actions without changing the underlying status language.
- Make ownership visible: who posted, who shortlisted, who interviewed, who uploaded, who accepted, and who still needs to act.

### Make pipeline status the organizing spine

In hiring, service, claims, and support workflows, users need to know where an item sits and what can happen next. A status-forward interface is often clearer than a feature-forward interface.

Design for:

- Stage visibility: applied, shortlisted, interview, hired, rejected, pending, active, closed.
- Upcoming work: interviews, invites, pending approvals, unsigned documents.
- Activity history: feedback, offer letter events, profile edits, document uploads.
- Recovery: rejected, incomplete, deactivated, missing document, expired invite, failed upload.
- Metrics that support decisions, not vanity: completion percent, shortlist count, interview count, hire count, rejection count.

### Keep AI assistance beside the artifact it changes

The resume-builder case studies show AI writing, job-description comparison, scoring, keyword suggestions, and resume review. The strongest transferable lesson is placement: assistance should sit close to the resume section or job criteria it affects.

For AI writing/review UI:

- Show the input source: job title, job description, LinkedIn/job URL, college code, selected resume section.
- Explain the evaluation basis: missing skills, grammar, passive voice, bullet quality, match category, resume completion threshold.
- Make suggestion scope explicit: experience, education, about, skills, job title, or full resume.
- Show selected suggestions and applied changes with a visible confirmation state.
- Handle no-score and low-data cases with a rule, not a vague failure message.
- Expose limits and upgrade prompts without interrupting the main editing flow.

### Let users explore before requiring commitment

For job search, public services, and marketplaces, login walls can weaken discovery. The Workruit examples include flows where users can leave onboarding and explore product opportunities before full sign-in.

Use this pattern when trust or fit is still unproven:

- Let visitors browse examples, jobs, events, datasets, or feature previews.
- Ask for account creation at the moment it protects progress or enables action.
- Preserve context after sign-in so the user returns to the item that motivated them.
- Make incomplete profiles useful but clearly limited.

### Turn uncertain search into guided discovery

The ICPSR case study framed a common search problem: users often do not know the exact term that will retrieve the right material. Semantic search can be ideal but expensive; UI can still help.

Feasible alternatives:

- Recommended datasets or items.
- Popular terms that behave like entry points, not decorative clouds.
- Category sections with plain-language labels.
- Breadcrumbs after drill-down.
- Search examples and query hints near the search box.
- Filters that reflect how users reason, not just database fields.

When the perfect intelligent feature is out of scope, identify the nearest interface-level improvement that reduces uncertainty now.

### Use technical feasibility as a design constraint early

ICPSR tested a synonym-like discovery idea and then deprioritized it because the needed data infrastructure was too heavy for the MVP. This is a useful lesson for AI, search, personalization, and automation work.

Before committing to a concept, ask:

- Does the organization already have the data required?
- Can the team maintain the taxonomy, model, or rules?
- Is the feature valuable enough to justify infrastructure work?
- What lighter UI pattern gives users similar confidence?
- What evidence would justify a later technical investment?

### Public portals need audience paths, not just a prettier homepage

The DEET redesign exposed a common landing-page issue: a single page was trying to serve job seekers, employers, partners, skill-development programs, job fairs, and public credibility.

For public service or marketplace landing pages:

- State who the page is for in the first viewport.
- Give each audience a clear path and CTA.
- Separate informational pages from conversion flows.
- Use product imagery or concrete examples to explain the service.
- Reduce decorative motion if multiple GIFs or animations compete with comprehension.
- Use testimonials, partner proof, event details, and FAQs where they reduce decision risk.

### Make institutional products feel credible, not merely modern

The ICPSR redesign improved search efficiency, then revisited visual design to increase professionalism and credibility. For academic, government, healthcare, financial, or data-heavy products, the tone should make users trust the system.

Credibility design moves:

- Consolidate confusing navigation.
- Use component patterns that can scale across future pages.
- Tune color saturation for legibility and authority.
- Use typography that supports the institution's context.
- Improve contrast and spacing without making the interface feel like a marketing template.
- Keep before/after comparisons tied to measurable task outcomes.

## Visuals Worth Inspecting

If working from the captured case studies or similar artifacts, inspect:

- Role-specific dashboards for employers and consultancies.
- Applicant cards showing profile completion, documents, interview state, and ownership.
- Activity and pipeline tabs that show stage transitions.
- AI resume score cards, suggestion cards, no-score states, and applied-suggestion confirmation.
- DEET landing-page explorations where CTA clarity, audience targeting, negative space, and distracting media are discussed.
- ICPSR before/V1/V2 comparisons showing discovery changes, navigation consolidation, and credibility polish.

Avoid copying the case-study presentation style directly. Extract the product patterns; many of the pages use oversized visual storytelling and repeated labels that are useful for portfolio narration but too heavy for production interfaces.

## Apply This In Practice

When designing these products, output:

- Roles and permissions.
- Shared objects and status model.
- Primary workflow per role.
- Discovery entry points for users who do not know exact terms.
- AI assistance boundaries and explanation.
- Empty, incomplete, failed, pending, and handoff states.
- Feasible MVP version and future intelligent version.
- Metrics to validate: task time, click-through, profile completion, application conversion, registration, bounce rate, time on page, support contacts, and successful handoffs.
