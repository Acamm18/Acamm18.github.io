## 2026-08-22 - CI/CD Efficiency via Paths Exclusions
**Learning:** In repositories with agent journals or internal tracking files (.jules/**), commits that only touch these files trigger full GitHub Pages deployments unnecessarily. Adding `paths-ignore: [".jules/**"]` to `.github/workflows/static.yml` avoids redundant build and deploy action runs.
**Action:** Always verify if non-production asset directories exist in the repo and ensure workflow triggers exclude them if they don't affect site contents.
