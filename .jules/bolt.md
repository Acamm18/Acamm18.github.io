## 2026-06-12 - CI/CD Optimization for Journal-Only Repos
**Learning:** In repositories like this one that lack application source code, traditional runtime optimizations aren't applicable. The primary performance lever is CI/CD efficiency. Using `paths-ignore` to exclude the agent journal directory (`.jules/**`) prevents redundant deployments and saves runner resources.
**Action:** Always check if a repository is primarily for documentation/logging and optimize the deployment triggers accordingly.
