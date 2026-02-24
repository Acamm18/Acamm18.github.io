# Bolt's Journal - Critical Learnings Only

## 2026-02-24 - Safe Concurrency Optimization for Static Sites
**Learning:** For GitHub Pages deployments using actions/deploy-pages, 'cancel-in-progress: true' is a safe and efficient optimization. Since the deployment is atomic and only the final state is relevant, cancelling redundant intermediate builds saves CI minutes and reduces deployment latency during rapid iterations.
**Action:** Always enable 'cancel-in-progress: true' for static site deployment workflows where intermediate states don't need to be preserved.
