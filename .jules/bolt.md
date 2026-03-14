## 2025-03-14 - GitHub Pages Deployment Optimization
**Learning:** In GitHub Pages repositories using `actions/deploy-pages`, enabling `cancel-in-progress: true` is a safe and effective optimization because deployments are atomic and only the latest state is relevant.
**Action:** Always check workflow concurrency settings for static deployments and enable `cancel-in-progress` to save runner minutes.
