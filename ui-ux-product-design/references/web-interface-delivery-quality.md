# Web Interface Delivery Quality

Treat performance, accessibility, and production delivery as user-experience behavior. Use the target project's budgets and checks first; apply these defaults only when the project has none.

## Performance as UX

- Target field LCP at or below 2.5 seconds, CLS at or below 0.1, and INP at or below 200 milliseconds.
- Use TBT below 200 milliseconds as a lab diagnostic target, not as field evidence.
- Distinguish Lighthouse's simulated lab result from CrUX or RUM data from real visits.
- Repeat noisy synthetic tests under the same conditions and use the median.
- Optimize a metric only after identifying the user-facing delay and its responsible resource or task.

## Critical rendering path

- Keep the LCP resource discoverable in initial HTML and give only that asset eager loading and high fetch priority.
- Do not lazy-load the LCP asset.
- Serve responsive modern images with correct intrinsic dimensions, `srcset`, and accurate `sizes`.
- Lazy-load secondary images and nonessential interface regions.
- Reserve image, video, iframe, and asynchronously inserted regions to prevent layout shift.
- Remove duplicate font sources and unnecessary render-blocking stylesheets before restructuring the whole style system.

## JavaScript and hydration

- Render static text, links, navigation, and content without client hydration.
- Hydrate immediately only when a control must work immediately.
- Hydrate secondary tools on visibility or interaction.
- Consolidate duplicate startup requests and reuse the first result.
- Trace forced reflow before editing. Batch layout reads and writes only when the trace identifies an attributable source.
- Do not add a dependency when native HTML, CSS, or browser APIs cover the behavior.

## Third-party functionality

- Do not request players, portals, widgets, or their preconnects before user intent unless they are essential to the primary task.
- Use an accessible normal link as the no-JavaScript fallback for a click-to-load facade.
- Load only the provider or instance the user activates.
- Load optional membership or account portal code on first pointer or keyboard intent; keep fallback links and expose ready, disabled, failure, and retry states.
- Preserve loading, disabled, success, failure, retry, and keyboard states.
- Reserve the facade's dimensions so activation does not shift surrounding content.
- Do not remove security, membership, consent, or recovery behavior solely to improve an audit score.

## Accessibility and agent browsing

- Prefer native `hidden`, `inert`, or DOM removal for inactive interactive regions.
- Never place focusable descendants inside `aria-hidden="true"` content.
- Keep duplicated marquees, tickers, carousels, and mobile menus out of the focus order when inactive or hidden.
- Preserve logical headings, landmarks, accessible names, contrast, focus order, and visible focus.
- Test the primary path with a keyboard and inspect the accessibility tree, not only the screenshot.

## Production and audit triage

- Test the final custom domain as well as localhost or a generated preview.
- Compare repository markup with the delivered response and network trace.
- Attribute injected scripts, deprecated APIs, headers, redirects, and `robots.txt` changes to the responsible application or edge layer.
- Fix an edge-generated failure at the edge; do not disguise it with unrelated application changes.
- Preserve correct high-DPR image selection when rendered size, device pixel ratio, `srcset`, and `sizes` justify the selected asset.
- Ignore diagnostics with zero estimated savings unless a trace or real user problem supplies evidence.
- Report what was measured, under which conditions, and what could not be verified.

## Authoritative references

- [Core Web Vitals workflows with Google tools](https://web.dev/articles/vitals-tools)
- [Optimize Largest Contentful Paint](https://web.dev/articles/optimize-lcp)
- [Lazy-load offscreen iframes](https://web.dev/articles/iframe-lazy-loading)
- [MDN: `aria-hidden`](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Reference/Attributes/aria-hidden)
- [Chrome Lighthouse: `robots.txt` is not valid](https://developer.chrome.com/docs/lighthouse/seo/invalid-robots-txt)
