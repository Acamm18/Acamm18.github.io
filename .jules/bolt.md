## 2025-02-25 - Safe Deployment Cancellation
**Learning:** In GitHub Pages deployments using `actions/deploy-pages`, `cancel-in-progress: true` is a safe optimization. Since the deployment process is atomic and only the latest state of the static site is relevant, canceling an older, still-running deployment in favor of a newer one saves CI/CD resources without risking site inconsistency.
**Action:** Always enable `cancel-in-progress: true` for static site deployment workflows to improve resource efficiency.
