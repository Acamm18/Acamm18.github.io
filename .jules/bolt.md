## 2026-07-02 - Optimize CI/CD by ignoring agent journals
**Learning:** Agent journaling in `.jules/` triggers unnecessary GitHub Pages deployments, consuming CI/CD resources for non-production changes.
**Action:** Use `paths-ignore: [".jules/**"]` in deployment workflows to exclude agent metadata from triggering production releases.
