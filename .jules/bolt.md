# Bolt's Journal ⚡

## 2026-02-19 - CI/CD Workflow Efficiency Optimization
**Learning:** In a static site repository with minimal assets, optimizing the CI/CD pipeline provides the most significant efficiency gains. Using `cancel-in-progress: true` prevents wasted compute on redundant deployments, and `paths-ignore` ensures that non-deployment changes (like journal updates) don't trigger unnecessary workflow runs.
**Action:** Always consider the cost of CI/CD triggers and redundant runs in automation-heavy environments.
