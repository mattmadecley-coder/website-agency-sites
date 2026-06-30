# website-agency-sites

Static hosting for lead sites built by Matthew's website-agency pipeline.

Each lead's site lives at `sites/<slug>/index.html` and is served by GitHub
Pages at:

    https://mattmadecley-coder.github.io/website-agency-sites/sites/<slug>/

Deployed automatically via GitHub Actions (`.github/workflows/deploy.yml`) on
every push to `main` — no build step, the workflow just uploads the repo
contents as-is. This replaced Netlify as the default lead-site host on
2026-06-30 once Netlify's credit-based Free plan (15 credits per production
deploy, 300/month hard cap) turned out unable to support the project's
50-sites/day target. Netlify is still used for the separate, low-volume
`agency-click-tracker` project — just not for lead sites anymore. See
`website-agency/RUNBOOK.md` in the main project repo for the full pipeline.
