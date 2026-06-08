## 2026-06-08 - CI/CD Optimization with paths-ignore
**Learning:** In repositories used primarily for agent journals and static site hosting, updates to the agent journal directory (.jules/) trigger redundant CI/CD runs.
**Action:** Always add 'paths-ignore: [".jules/**"]' to deployment workflows to save CI/CD resources and reduce noise.
