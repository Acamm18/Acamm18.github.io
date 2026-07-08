## 2026-07-08 - CI/CD Optimization via paths-ignore
**Learning:** In a GitHub Pages repository where the agent frequently updates journal files, the default deployment workflow triggers on every push, leading to redundant runner usage for non-production assets.
**Action:** Use `paths-ignore: [".jules/**"]` in the GitHub Actions workflow to exclude internal agent directories from triggering site deployments.
