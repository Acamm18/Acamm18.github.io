## 2026-03-15 - GitHub Pages CI/CD Efficiency
**Learning:** Enabling `cancel-in-progress: true` is safe for GitHub Pages deployments via `actions/deploy-pages` because they are atomic. Redundant runs for the agent journal (`.jules/**`) can be safely ignored to save runner minutes.
**Action:** Always check if `cancel-in-progress: true` and `paths-ignore` for non-functional files are implemented in deployment workflows.
