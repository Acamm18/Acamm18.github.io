
## 2026-07-13 - CI/CD Optimization with paths-ignore
**Learning:** In repositories dominated by agent journal entries and metadata, failing to exclude these paths from deployment workflows leads to redundant and wasteful CI/CD runs.
**Action:** Always verify if a repository has a dedicated metadata/journal directory (like `.jules/`) and ensure it is added to `paths-ignore` in the primary deployment workflows to save runner resources and reduce deployment noise.
