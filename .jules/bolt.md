# Bolt's Journal - Critical Learnings Only

## 2026-07-23 - Utilizing paths-ignore in Static Deployments
**Learning:** In production-sensitive deployment pipelines with explicit instruction warnings against canceling in-progress runs, we cannot use 'cancel-in-progress: true' to avoid redundant CI/CD execution. Instead, leveraging 'paths-ignore' for non-production agent metadata and journals under '.jules/**' is the optimal lever to reduce unnecessary builds and save GitHub Actions runner time.
**Action:** When working in repositories with deployment configurations and agent environments, prioritize 'paths-ignore' to restrict workflow execution only to production assets and source changes, thereby avoiding redundant pipeline runs safely.
