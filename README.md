# Pantry Ledger

A bilingual fictional pantry evidence ledger built with Next.js 16.3.8 and React.
Compare an original observation (six eggs) with its correction (two eggs), retain provenance and see how meal feasibility changes.

## Build and verify

Node 24. Install locked dependencies with `npm ci --ignore-scripts`, run `npm test`, then `NEXT_TELEMETRY_DISABLED=1 npm run build`.
`python3 scripts/prepare_release.py` prepares static assets with a restrictive Content Security Policy.
The complete current source is in `source.zip`. No Astro or Sanity Studio dependencies are part of this version.

## Data and current limits

Default data is a clearly labeled local fictional demo. The optional Load live button reads the public Sanity project `zmcwbews`, dataset `production`, without credentials. Twelve seed documents are prepared in `data/seed.ndjson`, but have not been imported. Empty or failed live queries show an error, never a false success.

Sanity data storage remains the intended backend. An authorized one-time content import is still required. This public viewer does not include a content editor, account login, write keys, analytics or stored personal information.

This is a preview, not a contest submission or a claim of award eligibility or earnings. Fictional meal quantities are software fixtures, not dietary or food-safety recommendations.
