## 2026-05-20 - CI/CD Optimization for Static Sites
**Learning:** In repositories used primarily for documentation or agent journaling, frequent updates to non-production assets can lead to excessive and redundant CI/CD runs.
**Action:** Always implement `paths-ignore` in GitHub Action workflows to exclude directories like `.jules/` that do not affect the production build, especially when explicit instructions forbid using `cancel-in-progress: true`.
