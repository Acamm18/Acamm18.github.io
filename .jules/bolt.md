## 2026-03-11 - Optimize GitHub Pages deployment workflow

**Learning:** In this repository, 'cancel-in-progress: true' is considered a safe optimization for the GitHub Pages deployment workflow because deployments via actions/deploy-pages are atomic and only the latest state is relevant for a static site. Additionally, using 'paths-ignore' for documentation directories prevents redundant CI runs.

**Action:** Always check if 'cancel-in-progress' can be enabled for deployment workflows and use 'paths-ignore' for non-application files to save CI resources.
