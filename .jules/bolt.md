## 2026-05-06 - CI/CD Optimization for Journal-only Repositories
**Learning:** In repositories primarily used for agent journaling (like this one), the primary performance bottleneck is the CI/CD pipeline. Every update to the journal triggers a full GitHub Pages deployment, which is redundant and consumes CI resources.
**Action:** Use `paths-ignore` in the workflow trigger to exclude `.jules/**` from triggering deployments, ensuring that meta-updates don't waste runner time.
