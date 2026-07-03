## 2026-07-03 - Workflow trigger optimization
**Learning:** In repositories with no application code and frequent agent journal updates, the CI/CD pipeline is the primary performance lever.
**Action:** Use 'paths-ignore' in GitHub Actions to prevent redundant deployments when updating documentation or agent-specific files like '.jules/**'.
