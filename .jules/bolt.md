## 2025-05-15 - Safe Deployment Cancellation
**Learning:** GitHub Pages deployments via `actions/deploy-pages` are atomic. The previous warning against `cancel-in-progress` in `static.yml` was unnecessary for this static site since only the latest state matters.
**Action:** Enable `cancel-in-progress: true` in deployment workflows for static sites to save CI resources during rapid iterations.
