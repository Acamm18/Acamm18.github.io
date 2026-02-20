## 2025-02-20 - GitHub Actions Workflow Optimization
**Learning:** Enabling `cancel-in-progress: true` for GitHub Pages deployments is a safe and effective way to save GitHub Actions resources, as only the latest site state is relevant. Additionally, using `paths-ignore` for non-deployment directories (like `.jules/`) prevents redundant builds.
**Action:** Always check GitHub Actions workflows for redundant triggers and enable `cancel-in-progress` when atomic deployments make it safe to do so.
