## 2026-05-08 - Optimizing CI/CD for Journal-Only Repositories
**Learning:** In repositories containing only GitHub Actions and agent journals (like .jules/bolt.md), every push triggers a deployment. Frequent journal updates lead to redundant runner usage and deployment churn.
**Action:** Use 'paths-ignore' to exclude the agent journal directory from deployment triggers, ensuring CI/CD resources are only used for actual site/workflow changes.
