## 2026-06-21 - CI/CD Optimization for Journal-only Repositories
**Learning:** In repositories like this one that primarily host metadata or journals (e.g., .jules/ directory) without application source code, the primary performance lever is CI/CD efficiency. Every push that only updates agent logs unnecessarily triggers a full GitHub Pages deployment.
**Action:** Use 'paths-ignore' in the deployment workflow to exclude non-production directories like '.jules/**' to save runner resources and reduce redundant deployments.
