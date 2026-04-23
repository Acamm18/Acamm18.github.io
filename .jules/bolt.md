## 2026-04-23 - CI/CD Optimization for Agent Journals
**Learning:** In repositories with agent journals (like `.jules/`), every update to a log file triggers a full deployment workflow. Since these files don't contribute to the site's content, these runs are redundant and consume CI resources.
**Action:** Always include `paths-ignore` for metadata or log directories in the primary deployment workflow to ensure only relevant changes trigger a build.
