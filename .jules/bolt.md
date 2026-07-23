## 2026-07-23 - [Static Workflow Deployment Filtering]
**Learning:** Updates to the agent journal directory `.jules/**` trigger unnecessary GitHub Pages workflow deployments on every commit. Since these files are internal tracking artifacts and are not part of the deployed static site, they consume unnecessary runner execution time and compute resource overhead.
**Action:** Configure the static deployment GitHub Action with `paths-ignore: [".jules/**"]` to prevent redundant workflows from running when only agent journals or tracking files are updated, saving CI/CD runner compute time.
