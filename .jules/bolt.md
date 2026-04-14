## 2026-04-14 - CI/CD Concurrency Constraints
**Learning:** The `.github/workflows/static.yml` contains an explicit developer warning against setting `cancel-in-progress: true` for GitHub Pages deployments. Although canceling redundant builds is a standard Bolt optimization, it must be avoided here to comply with the project's requirement for production deployments to complete.
**Action:** Focus on alternative CI/CD efficiency improvements such as `paths-ignore` for non-deployable assets (e.g., `.jules/**`) instead of modifying concurrency behavior.
