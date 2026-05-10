## 2026-05-10 - CI/CD Optimization for Journal-Heavy Repositories
**Learning:** In repositories primarily used for agent journals (like .jules/), frequent updates to these metadata files trigger unnecessary GitHub Actions runs, consuming runner minutes and cluttering deployment history.
**Action:** Always implement `paths-ignore` for non-production directories like `.jules/` in the deployment workflow to ensure that only relevant changes trigger a site rebuild.
