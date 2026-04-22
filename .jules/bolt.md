## 2026-04-22 - Optimize CI/CD by ignoring journal updates
**Learning:** Updates to the agent journal in `.jules/` do not affect the production site content but trigger redundant GitHub Pages deployment workflows, consuming CI/CD resources.
**Action:** Use `paths-ignore` in the GitHub Actions workflow configuration to exclude the `.jules/` directory from triggering deployments.
