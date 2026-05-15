## 2026-05-15 - Optimizing CI/CD for Journal-Only Repositories
**Learning:** In repositories where the primary activity is agent journaling and there is no application code, the most significant performance lever is the CI/CD pipeline efficiency. Preventing unnecessary deployments triggered by metadata or journal updates saves runner resources and reduces deployment noise.
**Action:** Always implement `paths-ignore` for non-production directories like `.jules/` in the deployment workflows of such repositories.
