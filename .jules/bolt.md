## 2026-07-07 - Optimize CI/CD with paths-ignore
**Learning:** In repositories where metadata or journal entries (like those in .jules/) are updated frequently but don't affect the site's content, the CI/CD pipeline triggers redundantly.
**Action:** Always check if certain paths (like journals or documentation) can be ignored in the deployment workflow to save runner resources.
