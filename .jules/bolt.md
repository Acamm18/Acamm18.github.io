# Bolt's Journal

## 2025-03-12 - Initializing Journal
**Learning:** Initialized the performance journal for the Acamm18.github.io repository.
**Action:** Follow the journal-based learning process.

## 2025-03-12 - CI/CD Optimization for Static Sites
**Learning:** In this repository, 'cancel-in-progress: true' is a safe optimization for the GitHub Pages deployment workflow because deployments via actions/deploy-pages are atomic and only the latest state is relevant for a static site. Additionally, using 'paths-ignore' for non-deployment directories like '.jules/' prevents redundant builds.
**Action:** Always check for 'cancel-in-progress' and 'paths-ignore' opportunities in CI/CD workflows for static sites to save resources.
