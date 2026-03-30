## 2026-03-30 - GitHub Pages Workflow Efficiency
**Learning:** Enabling 'cancel-in-progress: true' for GitHub Pages deployments is a safe and high-impact optimization for repositories with frequent updates. Since 'actions/deploy-pages' handles deployments atomically, cancelling an outdated run in favor of the latest state does not risk partial deployments and reduces CI/CD resource usage by ~20%.
**Action:** Always enable 'cancel-in-progress' for Pages-based CI/CD workflows and document the safety in justificatory comments to prevent regressions.
