## 2026-03-29 - GitHub Pages Deployment Optimization
**Learning:** In this repository, 'cancel-in-progress: true' is considered a safe optimization for the GitHub Pages deployment workflow because deployments via actions/deploy-pages are atomic and only the latest state is relevant for a static site.
**Action:** When working with GitHub Actions workflows in static site repositories, always check if 'cancel-in-progress' can be enabled to reduce redundant runs and save Actions minutes.
