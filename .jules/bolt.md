## 2026-07-15 - Optimizing GitHub Pages deployment triggers
**Learning:** In a pure configuration or journal-only repository, CI/CD pipeline efficiency is the primary performance lever. Excluding non-production assets like '.jules/**' using 'paths-ignore' prevents redundant workflow runs and saves runner resources.
**Action:** Always audit deployment workflows for 'paths-ignore' opportunities when introducing or maintaining agent-specific metadata directories.
