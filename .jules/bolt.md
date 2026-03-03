## 2025-03-03 - GitHub Pages Deployment Optimization
**Learning:** In the `static.yml` workflow, `cancel-in-progress` was initially set to `false` with a comment suggesting production deployments should complete. However, for GitHub Pages (especially static sites), deployments via `actions/deploy-pages` are atomic and only the latest state is relevant. Canceling stale runs saves CI minutes without risking site integrity.
**Action:** Always evaluate if `cancel-in-progress: true` is safe for the specific deployment target, even if comments suggest otherwise, provided the deployment is atomic.
