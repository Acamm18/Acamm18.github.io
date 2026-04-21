## 2026-04-21 - CI/CD Trigger Optimization
**Learning:** In repositories primarily used for agent journaling or configuration, standard CI/CD triggers on every push lead to redundant and inefficient deployments of static content when only meta-files (like `.jules/bolt.md`) are changed.
**Action:** Always implement `paths-ignore` for non-functional or meta directories (e.g., `.jules/**`) in deployment workflows to ensure resources are only spent on meaningful site updates.
