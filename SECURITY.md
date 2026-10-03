# Security scope — Next.js release, 2026-10-03

- This version replaces the previous Astro implementation. It does not include the previous Sanity Studio toolchain or any custom vendor security patches.
- The exact Next.js/React dependency lockfile was checked with npm audit: zero known advisories reported at the time of checking. This is a point-in-time dependency result, not a guarantee of zero vulnerabilities.
- Production output is static files only. No application server, account login, shared response cache, write token or mutation endpoint is deployed.
- Client connections are limited by Content Security Policy to the same origin and the named public Sanity API. Inline framework scripts receive exact content hashes.
- Data is rendered with React's ordinary text escaping. No user HTML is injected. No analytics or local browser storage is used.
- Public seed records are fictional. Known personal identifiers and key markers were excluded from the allowlisted release files.
- 28 data/functional tests passed. Next.js production build passed. Browser UI and live-data integration still require validation.
- Importing content or adding persistent account access is a separate owner-authorized step. Do not put credentials in this repository or website.
