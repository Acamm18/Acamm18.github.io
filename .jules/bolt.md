## 2025-03-09 - Safe Concurrency for Static Deployments
**Learning:** In repositories deploying static content via `actions/deploy-pages`, enabling `cancel-in-progress: true` is safe and highly efficient. Since deployments are atomic and only the final state matters, intermediate builds can be safely canceled without risking an inconsistent site state.
**Action:** Always enable `cancel-in-progress: true` for GitHub Pages static deployment workflows to save Action minutes and avoid redundant work.
