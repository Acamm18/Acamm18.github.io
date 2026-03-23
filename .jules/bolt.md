## 2025-03-23 - CI Workflow Efficiency
**Learning:** Updates to the agent journal (`.jules/`) trigger full GitHub Pages deployments, consuming CI minutes for non-production changes.
**Action:** Use `paths-ignore` in the workflow trigger to exclude the `.jules/` directory.
