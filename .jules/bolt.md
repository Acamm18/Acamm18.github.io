## 2026-04-15 - Optimizing CI/CD for Journal-Heavy Repositories
**Learning:** In repositories like this one, where the primary activity is agent logging and the codebase is minimal, CI/CD efficiency becomes the most impactful performance lever. Ignoring path updates that don't affect the production environment (e.g., `.jules/**`) prevents redundant GitHub Actions runs and saves runner resources.
**Action:** Always verify if high-frequency file updates (like logs or journals) should trigger a full deployment. Apply `paths-ignore` to those directories in the CI/CD configuration.
