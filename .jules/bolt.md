## 2026-07-10 - Optimizing CI/CD by ignoring agent journal updates
**Learning:** Frequent updates to internal agent journals (`.jules/`) trigger unnecessary GitHub Actions runs for GitHub Pages deployments, wasting runner minutes.
**Action:** Always add `paths-ignore: [".jules/**"]` to deployment workflows in repositories where Bolt or other agents maintain persistent journal files.
