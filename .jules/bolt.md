## 2026-04-24 - Optimize CI/CD by ignoring journal updates
**Learning:** Updates to agent journal files in `.jules/` trigger full GitHub Pages deployments, even though these files are not part of the site's content. This leads to redundant CI/CD runs and wasted runner resources.
**Action:** Use `paths-ignore` in the GitHub Actions workflow to exclude the `.jules/` directory from triggering deployments, ensuring runs only occur for relevant site changes.
