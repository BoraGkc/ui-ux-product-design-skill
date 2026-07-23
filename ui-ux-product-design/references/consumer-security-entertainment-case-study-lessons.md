# Consumer Security, Entertainment, and Booking Case Study Lessons

Read this when the task involves home cybersecurity, parental controls, IoT/device monitoring, event discovery, ticketing, seat maps, cinema showtimes, curated streaming, film/social entertainment apps, partner self-serve tools, access management apps, portfolio/content discovery, or consumer products that need to turn complex inventory or invisible risk into simple action.

Source creator: [Karolis Kosas](https://karoliskosas.com/). Original pages remain authoritative for project roles and collaborators.

Sources reviewed:

- CUJO: https://karoliskosas.com/cujo-3/
- YPlan: https://karoliskosas.com/yplan-2/
- Cinema Club: https://karoliskosas.com/cinemaclub/
- Rapt Studio: https://karoliskosas.com/rapt/
- MUBI: https://karoliskosas.com/mubi-5/

## Contents

- Transferable Lessons
- Visuals Worth Inspecting
- Apply This In Practice

## Transferable Lessons

### Make invisible security answerable

CUJO translated abstract home cybersecurity into three concrete user questions: whether the home is exposed to threats, which devices are active, and what children are doing online. This made the app architecture easier to understand.

For security and network products:

- Start from questions users naturally ask, not from technical features.
- Group around mental models: threats, devices, parental controls, overview.
- Show device identity clearly, including obscure IoT devices.
- Make threat summaries reassuring and actionable instead of frightening.
- Use cards for scalable overview data when new security features will be added over time.

### Design parental controls around family routines

CUJO's parental controls became clearer when schedules mapped to routines like homework and bedtime. Families often need different rules for different ages, devices, and times of day.

Useful patterns:

- Profiles for each child or household member.
- Schedule cards tied to recognizable routines.
- One-tap editing for time, days, and restrictions.
- Age-appropriate defaults with room for customization.
- Usage summaries that explain time, categories, threats, and most visited sites.
- Setup funnels optimized for completion, not maximum configurability on step one.

### Turn power users into a community signal

CUJO found that security-aware users wanted to report threats. The Cyber Neighborhood Watch pattern turned individual reports into a visible shared feed and back-end review pipeline.

Use this carefully when:

- Users have expertise or motivation to contribute.
- Reports can be reviewed before affecting others.
- Contributions build trust and collective value.
- The UI distinguishes user reports, verified threats, and system action.

### Bounded inventory needs multiple discovery modes

YPlan began as a curated daily shortlist, then needed web and app surfaces that supported more inventory, search acquisition, expensive events, and advance planning. Less inventory is not always simpler if it blocks a user's real intent.

Match the discovery model to the job:

- Spontaneous last-minute browsing: curated feed and lightweight checkout.
- Planned theatre booking: date flexibility, seat maps, price comparison, rich metadata.
- Specific lookup: search, category, date, location, and venue filters.
- Ticket ownership/on-site use: tickets and admission flows must be easy to find.

### Separate filters from sorting by how users reason

YPlan distinguished unambiguous properties from ranking preferences. Category and date work well as filters; best match, popularity, distance, and price may be better as sorting or range controls depending on intent.

Use:

- Filters for exact constraints.
- Sorting for ranking criteria.
- Ranges for price, distance, and time.
- Clear defaults based on the most common use case.
- Secondary controls that support navigation rather than compete with it.

### Design marketplace supply tools for simple and complex sellers

YPlan's event organizers split into two groups: those wanting flexible power and those wanting minimum effort. A self-serve platform had to support both one-off events and complex recurring schedules.

For partner/supply-side tools:

- Start with the simplest event setup that covers most cases.
- Add vertical-specific complexity only after observing partners.
- Prototype with real organizers using rough interactive flows.
- Use visual overviews for date/time/ticket complexity.
- Provide performance overview and ticket management on desktop and mobile.
- Design access management for noisy, time-pressured entrance environments.

### Optimize admission tools for the physical context

Access management at live events happens under pressure, noise, poor lighting, and queues. YPlan's access app used bold colors and gestural swiping because the job was physical, not desk-bound.

Consider:

- Large targets and high contrast.
- Fast accept/reject gestures.
- Offline or sync resilience when possible.
- Real-time link to event data.
- Minimal text at the point of entry.

### Design cinema discovery around film and venue intents

Cinema Club learned that users usually searched either for a specific film or a specific cinema. Those became the main architecture rather than a generic popularity list.

For showtime products:

- Treat film pages and cinema pages as primary touchpoints.
- Strip film/cinema metadata to essentials when the task is finding showtimes.
- Use cards to group dense showtime information.
- Default to distance when nearby attendance matters.
- Offer alternative sorting for "soonest nearby," price, time, preferred chain, or favorite venue.
- Let users save favorite cinemas because venue loyalty is a real behavior.

### Use favorites as meaningful personalization input

Cinema Club used favorite cinemas to personalize feeds, shortcuts, and notifications. This is stronger than asking for vague preferences because it reflects a real repeated behavior.

Good personalization inputs:

- Favorite venues.
- Saved films/events.
- Past bookings.
- Preferred time windows.
- Price sensitivity.
- Nearby/work/home context when permissioned.

### Work around fragmented booking constraints honestly

Cinema ticketing involved fragmented chains and limited third-party access. Cinema Club used vouchers and a simplified two-step booking flow where direct seat booking was not available.

When supply constraints block the ideal flow:

- Explain what the user is actually buying.
- Do not imply a seat is guaranteed if it is not.
- Reduce steps where the system has supply access.
- Use price/distance visualization to help users choose.
- Keep the workaround visibly useful rather than pretending the constraint does not exist.

### Design retention experiments around real social behavior

Cinema Club observed that people shared screenshots of showtimes in chats. A chat-optimized sharing flow was more aligned with real planning behavior than a generic share button.

For retention and social planning:

- Observe how users coordinate outside the app.
- Make share artifacts useful in the destination context.
- Encourage the first transaction when repeat behavior depends on it.
- Test habit loops around weekly discovery or upcoming releases.

### Use curation as a product constraint

MUBI's limited catalog is a product promise: fewer films, stronger taste, less browsing bloat. Curated entertainment products should turn constraints into confidence.

Design implications:

- Explain why the catalog is limited.
- Make each item feel selected, not merely available.
- Support social or critical context for discovery.
- Preserve cross-platform consistency across mobile, TV, and console surfaces.
- Keep browsing lightweight while giving film lovers enough depth to trust the selection.

### Make portfolio/content sites easier to maintain and explore

Rapt Studio focused on content strategy, discoverability, and update flow for a large body of work and thought leadership. A visually impressive studio site still needs information architecture that helps visitors find work and lets teams maintain it.

For portfolio, agency, or thought-leadership sites:

- Separate work items, thought items, and service/brand story.
- Design update workflows, not only public pages.
- Use content strategy to decide what gets featured, grouped, and archived.
- Increase discoverability without flattening the brand's expressive voice.

## Visuals Worth Inspecting

If working from the captured pages or similar artifacts, inspect:

- CUJO's tab architecture, threat/device/parental control cards, schedule controls, profile usage summaries, icon system, and design system components.
- YPlan's web event pages, checkout flows, app navigation, filters/sorting, theatre seat maps, partner event setup, Trello-like ticket/date grid, and access management app.
- Cinema Club's film/cinema architecture, showtime cards, date picker, favorite cinema shortcuts, price/distance visualization, voucher checkout, chat sharing, and retention experiments.
- Rapt Studio's work/thought discovery and content maintenance patterns.
- MUBI's limited-catalog positioning, social film network, mobile app, and TV/console app considerations.

## Apply This In Practice

When designing or reviewing these products, output:

- Primary user questions or intents.
- Inventory model and discovery modes.
- Filter/sort/range rules.
- Booking or setup flow variations for simple vs complex cases.
- On-site or physical-context constraints.
- Personalization inputs and privacy notes.
- Community/reporting contribution model.
- Design system components for cards, lists, schedules, filters, tickets, profiles, and status.
- Metrics to validate: MAU, retention, conversion, checkout completion, setup completion, self-serve partner adoption, ticket scan speed, repeat booking, subscriber conversion, content discoverability, and support load.
