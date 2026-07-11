## 2026-07-11 - Prevent unnecessary deployments from agent journal updates
**Learning:** Updating the agent's journal in `.jules/` triggers a full GitHub Pages deployment, which is unnecessary and consumes CI/CD resources.
**Action:** Use `paths-ignore: [".jules/**"]`, in the GitHub Action trigger to exclude these files from deployment triggers.
