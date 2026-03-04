## 2025-03-04 - Optimize GitHub Pages Deployment Workflow
**Learning:** In repositories where an agent frequently updates logs or journals (like `.jules/`), failing to ignore these paths in the deployment workflow leads to redundant CI/CD runs. Additionally, for static site deployments, `cancel-in-progress: true` is a safe optimization as only the latest state is relevant.
**Action:** Always check for agent-specific directories and ensure they are ignored by deployment triggers. Enable `cancel-in-progress: true` for deployment-focused workflows to save resources.
