## 2026-06-29 - CI/CD Optimization: Ignore journal updates
**Learning:** Updates to the agent journal in .jules/ trigger full GitHub Pages deployments even though they don't affect the live site. This wastes GitHub Actions runner minutes and creates unnecessary deployment history.
**Action:** Use paths-ignore in GitHub Action workflows to exclude non-production assets and directories like .jules/ from triggering production deployments.
