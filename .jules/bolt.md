## 2025-05-14 - Optimize CI/CD workflow for static site
**Learning:** For static site deployments via `actions/deploy-pages`, enabling `cancel-in-progress: true` is a safe optimization because the deployment is atomic and only the latest state matters.
**Action:** Always enable `cancel-in-progress` in static site workflows and ignore non-source paths like `.jules/**` to save Action minutes.
