# ACOA Van Dashboard

Public dashboard of the Amesbury Council On Aging van program's ridership and cashflow. It is published at https://acoa-van.dwjellison.workers.dev (Cloudflare Worker) and mirrored at https://djellison.github.io/acoa-van/ (GitHub Pages).

- See `README.md` for the data definitions (Needs vs Social, net cashflow) and update steps.
- `index.html` uses d3 and recalculates everything from `data/*.csv` when it loads. Keep the CSV columns unchanged.
- Never include driver notes or rider personal information. The site is public.
- Cloudflare serves the repo root as static assets (`wrangler.jsonc`). Files listed in `.assetsignore` are not published, so add any new non-site file there.
- This is a git repo. Commit only when asked. A push to `main` publishes the live site: Workers Builds redeploys Cloudflare and GitHub Pages rebuilds.
- To deploy by hand without pushing, run `wrangler deploy` (wrangler is installed globally).
