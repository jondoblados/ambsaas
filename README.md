# ambsaas — POC2 publisher

Publishes **https://jon.doblados.net/ambsaas/**: the AMBSAAS website proof of concept 2, where the site is a
Next.js app (static export) and content is still edited in Google Docs.

This repository only holds the deploy workflow (`.github/workflows/deploy.yml`). GitHub Pages serves a repository
named `ambsaas` at `/ambsaas/` on the `jon.doblados.net` user site.

- Website code: [`jondoblados/poc` branch `poc2`](https://github.com/jondoblados/poc/tree/poc2) (see its README)
- Content: `content/` + `data/` from [`jondoblados/poc` branch `main`](https://github.com/jondoblados/poc), which the
  POC1 workflow updates from the Google Drive LIVE folder
- Runs every 15 minutes 08:00-24:00 SGT (skips when nothing changed), daily at 00:10 SGT, or via **Run workflow**
- `/ambsaas/build.json` shows which code and content commits are live
