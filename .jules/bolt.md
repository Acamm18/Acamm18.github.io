## 2026-11-02 - CI/CD Pipeline Bottleneck from Agent Journaling
**Learning:** In static GitHub Pages repositories without application source code, agent tracking and journal updates to `.jules/**` trigger redundant GitHub Actions deployment runs, consuming CI/CD runner minutes and runner queue capacity.
**Action:** Configure `paths-ignore: [".jules/**"]` on push triggers in `.github/workflows/static.yml` to prevent non-production documentation updates from triggering deployments.
