# QuantumSolar.ai — coming-soon site

Single static page (`index.html`), deployed on Netlify, domain on GoDaddy.

## Lead capture
Netlify Forms (native). Submissions: Netlify dashboard → Site → **Forms** → `waitlist`
(email + role). Turn on email notifications under Forms → Notifications.

## Analytics
Google Analytics 4. Replace `G-PLACEHOLDER` (2 occurrences in `index.html`)
with the Measurement ID from analytics.google.com for quantumsolar.ai.
Custom event `waitlist_signup` fires per signup with the visitor's role.

## Deploy
Every push to `main` auto-deploys via Netlify's GitHub integration.

## DNS (GoDaddy → Netlify)
- `A` record: `@` → `75.2.60.5`
- `CNAME`: `www` → `<site-name>.netlify.app`
(Authoritative values: Netlify dashboard → Domain settings.)

(Form detection enabled 2026-08-20 — this commit triggers the registering deploy.)
