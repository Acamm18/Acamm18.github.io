## 2025-05-15 - GitHub Pages Workflow Optimization
**Learning:** Enabling `cancel-in-progress: true` is safe for GitHub Pages deployment workflows because `actions/deploy-pages` is atomic; only the final state is relevant, and intermediate deployments are redundant. Additionally, `paths-ignore` for agent-specific directories prevents wasted build minutes.
**Action:** Always enable `cancel-in-progress` and ignore non-site paths (like `.jules/`) in static site deployment workflows.
