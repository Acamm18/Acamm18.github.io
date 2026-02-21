## 2026-02-21 - Workflow optimization for GitHub Pages
**Learning:** GitHub Pages deployments via `actions/deploy-pages` are atomic. Therefore, `cancel-in-progress: true` is a safe and efficient optimization to save GitHub Actions runner minutes when multiple pushes occur in quick succession. Additionally, using `paths-ignore` for non-deployment files like journals avoids unnecessary workflow runs.
**Action:** Updated `static.yml` to enable `cancel-in-progress: true` and added `paths-ignore` for `.jules/**`.
