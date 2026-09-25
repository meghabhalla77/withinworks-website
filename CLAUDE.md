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
