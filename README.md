# Samgori Solutions

Static website for Samgori Solutions: NetSuite post-implementation services.

Site files are in `public/`; `wrangler.jsonc` tells Cloudflare to serve that folder.

Pages: `index.html` (Home), `services.html`, `portfolio.html`, `about.html` (About, resume and contact form). Shared styles are in `public/styles.css`.

The contact form in `public/about.html` needs an email-forwarding endpoint to send mail. Set `FORM_ENDPOINT` (and `ACCESS_KEY` if the service needs one) in the script at the bottom of that file. Until then it shows a copy-and-email fallback.
