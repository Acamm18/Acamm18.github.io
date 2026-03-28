## 2026-03-28 - Optimizing GitHub Pages Deployment Concurrency
**Learning:** Enabling `cancel-in-progress: true` for GitHub Pages is a safe and effective way to reduce redundant Action runs because deployments via `actions/deploy-pages` are atomic. Only the latest state matters for a static site.
**Action:** Always check `concurrency` settings in deployment workflows to ensure we aren't wasting resources on obsolete runs.
