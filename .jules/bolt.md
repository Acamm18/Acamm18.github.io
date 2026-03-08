## 2026-03-08 - GitHub Actions Optimization
**Learning:** For static site deployments via `actions/deploy-pages`, `cancel-in-progress: true` is safe and efficient because deployments are atomic. Additionally, ignoring agent-specific directories (`.jules/**`) in push triggers prevents redundant CI runs.
**Action:** Always check for `cancel-in-progress` and `paths-ignore` opportunities in CI/CD workflows for static sites.
