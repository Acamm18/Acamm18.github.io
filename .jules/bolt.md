
## 2026-09-04 - Workflow Trigger Optimization
**Learning:** In repositories containing only deployment workflows and agent journals, adding `paths-ignore: ['.jules/**']` under the push trigger prevents redundant CI/CD builds and saves runner minutes whenever internal journal entries are updated.
**Action:** Always verify that internal agent/documentation paths are excluded from static site deployment triggers when configuring GitHub Actions workflows.
