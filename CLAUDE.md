# WithinWorks Leadership website

Marketing site for Megha Bhalla's leadership coaching practice. Plain static site: no framework, no build step.

## Files
- `index.html` — the whole site. Sections in order: hero, about, process, services, faq, blog, contact.
- `style.css` — all styles. Fonts: Fraunces (headings) and Jost (body) from Google Fonts.
- `script.js` — small interactions (nav, FAQ toggles, scroll effects).
- `assets/` — logo, portrait, meeting photo, partner logos.
- `BRAND-BRIEF.md` — approved copy and brand facts. Quotes marked verbatim must not be reworded.
- `content-drafts/` — blog article drafts in Markdown. Not published yet.

## Hosting and deploys
- Hosted on Vercel, project `withinworks-website`. Domain: withinworksleadership.com (registered at GoDaddy).
- Production deploys from the `main` branch. Merging to main publishes the site.
- Preview locally with `npx serve -l 5500 .` and open http://localhost:5500.

## Working rules
- Megha is the owner and is non-technical. Explain changes in plain language and show her a preview link before merging.
- Keep it simple: one HTML file, no frameworks, no dependencies unless there is a clear need.
- Booking goes through Calendly; WhatsApp link is in the contact section. Keep both working.
- Stripe payments are planned. Prefer Stripe Payment Links or hosted Checkout so no backend is needed.

## Pending setup
See `NEXT-STEPS.md`. If it has unchecked items, offer to guide Megha through the current step.

## Improvement backlog
See `AUDIT-CHECKLIST.md`. When Megha asks what to work on next, start there and update the checkboxes as items are completed.

## How to work with Megha (manage upward)
Megha is the business owner, not the operator. Bring her only decisions that
add impact or value to the business, affect go-to-market, or are dependencies
for those (pricing, offers, testimonials, positioning, partnerships, launches,
anything that needs her identity or money: Stripe, Vercel ownership, domain).

Do not bring her day-to-day work: code, layout, images, SEO plumbing, tooling,
deploys, copy tweaks. Handle those yourself or leave a note for Sahil (the
builder) in `NEXT-STEPS.md` under a "For Sahil" heading.

When she asks "what should I do next", give her at most three items, ranked by
business impact, each with why it matters and exactly what you need from her.
Batch small asks into one sitting rather than dripping them.

The research in `AUDIT-CHECKLIST.md` and future research files is the shared
brain. Sahil keeps adding to it. Read it before proposing work.
