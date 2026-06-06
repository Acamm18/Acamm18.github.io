## 2026-06-06 - CI/CD Optimization via Path Filtering
**Learning:** In metadata-heavy or journal-centric repositories, GitHub Actions workflows often trigger redundantly for non-functional changes. Using `paths-ignore` for directories like `.jules/` is a high-impact, low-risk efficiency win.
**Action:** Always audit workflow triggers for exclusion opportunities when working in repositories with significant documentation or agent-specific metadata.
