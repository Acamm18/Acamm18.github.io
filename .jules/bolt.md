## 2025-05-14 - Optimizing GitHub Pages Deployment Efficiency

**Learning:** In a repository primarily used for static hosting with frequent agent interactions (like this one), many CI/CD runs are triggered by metadata or journal updates that don't affect the site's content. Additionally, since GitHub Pages deployments are atomic, multiple concurrent deployments for the same branch are redundant.

**Action:** Optimized the deployment workflow by adding `paths-ignore` for agent-specific directories and enabling `cancel-in-progress: true` in the concurrency configuration. This reduces compute usage and ensures only the latest version is deployed.
