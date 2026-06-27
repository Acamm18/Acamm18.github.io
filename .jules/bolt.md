## 2026-06-27 - [CI/CD Optimization: Ignoring Metadata Updates]
**Learning:** In repositories where agent journals or metadata are stored alongside the source code, every agent interaction can trigger unnecessary CI/CD runs.
**Action:** Use 'paths-ignore' in GitHub Actions to exclude non-production directories like '.jules/' from triggering deployment workflows.
