# Samgori Solutions

Static website for Samgori Solutions: NetSuite post-implementation services.

Site files are in `public/`; `wrangler.jsonc` tells Cloudflare to serve that folder.

Pages: `index.html` (Home), `services.html`, `portfolio.html`, `about.html` (About, resume and contact form). Shared styles are in `public/styles.css`.

The contact form in `public/about.html` submits to a HubSpot form ("Website Contact Form") through HubSpot's form submission API. Each submission creates a contact in HubSpot and emails a notification to maia.eliozashvili@samgorisolutions.com. The portal and form IDs are set at the top of the script at the bottom of that file. If sending fails, the form shows a copy-and-email fallback.
