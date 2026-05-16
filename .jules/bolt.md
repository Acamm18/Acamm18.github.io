## 2026-05-16 - Optimize deployment triggers with paths-ignore
**Learning:** In repositories primarily used for agent activity or documentation, excluding non-production paths (like `.jules/**`) from deployment workflows significantly reduces redundant GitHub Actions runs and conserves runner resources.
**Action:** Always check if there are specific directories that don't contribute to the deployed site and exclude them from the push trigger using `paths-ignore`.
