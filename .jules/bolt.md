# Bolt's Journal ⚡

## 2025-05-14 - Initial Setup
**Learning:** Found that the repository is a minimal GitHub Pages site with only a deployment workflow.
**Action:** Identified opportunities to optimize the CI/CD workflow by cancelling in-progress runs and ignoring non-deployment files.

## 2025-05-14 - Workflow Optimization
**Learning:** In a static site deployment, only the latest state matters. Cancelling in-progress builds for older commits is a safe way to save CI resources.
**Action:** Always check `cancel-in-progress` and `paths-ignore` in GitHub Actions workflows for static sites.
