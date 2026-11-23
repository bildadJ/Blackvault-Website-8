# Blackvault: cinematic Group website (repository)

Upload the CONTENTS of this folder to the root of a GitHub repository. Cloudflare serves every file here to the public, so keep private documents out of it.

## Pages
- index.html: Blackvault Group (welcome sequence, vault door, custom menu, the first door to Agri Ventures, the doors ahead, capital philosophy and pipeline, intelligence, governance and contact)
- agri.html: Blackvault Agri Ventures (cinematic page: produce, branded truck, seed-to-shelf story, farm hubs, order and visit requests)
- verify.html, briefing.html, 404.html: utility pages (document verification, newsletter confirmation, not found)

## Files (all names are lowercase and must stay that way)
- assets/style.css and assets/app.js: Group site
- assets/agri-cinema.css and assets/agri-cinema.js: Agri Ventures page
- assets/api.js: API address and Turnstile site key. KEEP YOUR EXISTING assets/api.js if it already holds your real key.
- assets/verify.js, briefing.js, app404.js: utility pages
- assets/logo-lockup.svg, logo-mark.svg (Blackvault); agri-lockup.svg, agri-mark.svg, agri-favicon.svg (Agri Ventures logo)
- assets/photos: put real photographs here (see README.txt). The Agri page ignores missing photos.
- _headers: security headers. Scripts and styles live in files because the policy blocks inline scripts.

## Before launch
1. Check assets/api.js has your Turnstile site key (not the placeholder).
2. Add the registration number and registered address on the Governance and contact section when confirmed.
3. Deploy: Cloudflare Workers and Pages > connect this repository > build command empty > output directory / (or blank).
