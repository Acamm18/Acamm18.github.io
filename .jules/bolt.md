## 2026-07-04 - CI/CD Optimization for Journal Updates
**Learning:** In repositories where agent journals are updated frequently, CI/CD pipelines can be triggered unnecessarily, wasting resources.
**Action:** Use `paths-ignore` in GitHub Action workflows to exclude the journal directory (e.g., `.jules/**`) from deployment triggers.
