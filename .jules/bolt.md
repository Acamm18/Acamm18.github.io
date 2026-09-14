## 2026-09-14 - Ignore Non-Production Agent Files in Deployment Workflows
**Learning:** Updates to agent journal files (like .jules/bolt.md) trigger full GitHub Pages static deployment workflows unnecessarily when paths-ignore is not configured.
**Action:** Add paths-ignore: [".jules/**"] to static deployment workflows to eliminate redundant CI/CD runs and conserve GitHub Actions runner minutes.
