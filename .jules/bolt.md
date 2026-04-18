## 2026-04-18 - CI/CD Optimization for Journal Updates
**Learning:** Frequent updates to the agent journal in `.jules/` triggered redundant GitHub Pages deployments, wasting CI/CD resources and cluttering the Actions log.
**Action:** Implement `paths-ignore` for `.jules/**` in the deployment workflow to ensure the site only redeploys when actual content or configuration changes.
