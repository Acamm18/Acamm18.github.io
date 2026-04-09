## 2026-04-09 - Workflow trigger optimization for agent activity
**Learning:** Updates to the agent's journal (`.jules/bolt.md`) were triggering full GitHub Pages deployments, wasting CI/CD resources for documentation-only changes.
**Action:** Use `paths-ignore` in GitHub Actions workflows to exclude agent-specific directories from deployment triggers when those directories don't contain static assets.
