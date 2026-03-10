## 2025-03-10 - Optimizing CI/CD for Agent Journals
**Learning:** In a repository primarily used for agent activities and GitHub Pages hosting, frequent updates to agent journals (like `.jules/bolt.md`) can trigger unnecessary and resource-intensive deployment workflows.
**Action:** Always add `paths-ignore` for metadata or journal directories (like `.jules/**`) in the deployment workflow triggers. Also, set `cancel-in-progress: true` for static site deployments to ensure only the latest state is processed, saving Actions minutes.
