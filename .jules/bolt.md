# Bolt's Journal ⚡

## 2025-02-18 - CI/CD Workflow Efficiency Optimization
**Learning:** For a repository that primarily serves as a GitHub Pages site with minimal assets, the most significant performance gains come from optimizing the CI/CD pipeline. Unnecessary workflow runs and redundant deployments waste GitHub Actions resources and increase the time to see the latest changes in a concurrent push scenario.
**Action:** Implement `cancel-in-progress: true` for deployments and use `paths-ignore` to prevent non-functional changes from triggering expensive CI/CD runs.
