## 2026-04-19 - CI/CD Optimization for Journal Updates
**Learning:** Updating agent-specific files like `.jules/bolt.md` triggered full site deployments to GitHub Pages, which is inefficient since these files do not affect the public site content.
**Action:** Use `paths-ignore` in the GitHub Actions workflow to prevent deployments when only internal agent documentation is modified.
