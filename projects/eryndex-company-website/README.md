# ERYNDEX — Company Website

Responsive bilingual (English/Persian) company website and engineering portfolio.

## Preview
- English: https://eryndex.net/
- Persian: https://eryndex.net/fa/

## Structure
- `index.html` — English homepage
- `fa/index.html` — Persian homepage
- `services/` — dedicated service pages
- `work/` — selected project case studies
- `assets/style.css` — shared responsive styles
- `assets/script.js` — navigation, scroll progress and inquiry-form client logic
- `contact-api/` — Cloudflare Worker source for server-side inquiry delivery

## Portfolio positioning
The projects displayed on the website are engineering portfolio demonstrators maintained in the repository under `projects/`. They are included to make implementation samples available for review. They must not be described as customer deployments or production systems unless that status is independently verified. Each project README is the source of truth for implemented features and known limitations.

## Contact form status
The contact form interface and validation are present. Until the Worker is deployed, configured with secrets and tested, submissions fall back to opening the visitor's email application. The online form is **not yet a live server-side submission service**. Follow `contact-api/README.md`.

GitHub Pages is static hosting. It does not run the Worker or allow arbitrary HTTP response headers. The current HTML Content Security Policy is a partial browser-side control, not a replacement for server response headers. For production, place the site behind a host/CDN that can enforce security headers, configure rate limiting and bot protection, and test the deployed configuration.

## Before production launch
1. Deploy and test the contact Worker, configure a verified sender domain and store provider credentials as Worker secrets.
2. Add rate limiting and bot protection, and confirm the privacy notice and retention policy.
3. Configure production security response headers and HTTPS at the hosting/CDN layer.
4. Audit all service claims and project case studies against code and tests.
5. Confirm brand/legal identity and publish legal details only after formal verification.

The site is plain HTML, CSS and JavaScript and requires no frontend build step.
