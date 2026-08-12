# Hosting Notes — Neil Panchal

## Why GitHub Pages is the default

FireSafe Atlas is planned as a static dashboard: HTML, CSS, JS, and pre-exported data files (GeoJSON, CSV, images). A static site does not need a server running all the time, a database, or any backend logic. GitHub Pages serves exactly that kind of site directly from this repository, for free, with no billing account and no separate infrastructure to maintain.

Using GitHub Pages also matches the project's continuity rule: the dashboard has to keep running after any intern leaves, from the Seaside/Rhea-owned repository, not from anyone's personal laptop or account. GitHub Pages publishes straight from the repo's `main` branch, so as long as the repo exists, the site exists. A VM tied to one person's account would break that rule.

Once `dashboard/index.html`, `dashboard/styles.css`, `dashboard/app.js`, and the data files are in place, publishing is a Settings change (Pages → Deploy from a branch → `main` → `/root`), covered in `deployment/github-pages.md`.

## When a free VM would actually be needed

A VM (or similar backend hosting) only becomes necessary if the project adds something GitHub Pages cannot do on its own:

- User accounts or logins
- File uploads from site visitors
- A live, writable database
- Server-side GIS processing (something heavier than what a browser can run)
- Scheduled jobs that refresh data automatically without a person re-exporting files
- Private API keys that cannot be safely exposed in browser-side JavaScript

None of these are part of the Phase 1 dashboard plan. Fire, population, and boundary data are exported as static files by hand (or by a periodic manual process), not pulled live by a server.

## What happens if a VM is needed later

If the project does grow into one of the cases above, the next step is a written comparison of free-tier options (GitHub Pages vs. Cloudflare Pages vs. Oracle Cloud Always Free vs. Google Cloud Free Tier) before anything is created, and no VM, cloud account, or billing resource gets created without approval from Rhea Ghosal and Catherine Mudd. This week is research only — no accounts have been created.

## Summary

GitHub Pages is sufficient for the FireSafe Atlas dashboard as currently scoped. Revisit this decision only if the dashboard needs live backend functionality beyond serving static files.
