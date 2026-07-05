## 2026-07-05 - Optimize deployment workflow with paths-ignore
**Learning:** In repositories primarily used for agent tracking or static content where certain directories (like `.jules/`) are frequently updated but don't impact the live site, omitting these paths from the deployment trigger reduces redundant GitHub Actions runs.
**Action:** Always audit workflow triggers and use `paths-ignore` for internal or non-production assets to optimize CI/CD resource usage.
