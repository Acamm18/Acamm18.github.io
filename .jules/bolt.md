## 2026-05-13 - CI/CD Optimization for Agent Journals
**Learning:** In repositories consisting primarily of GitHub Pages deployments and agent journals (without application source code), CI/CD pipeline efficiency is the primary performance lever. Using `paths-ignore` for non-production assets like journal files prevents redundant deployment runs.
**Action:** Always check if agent journal directories (e.g., `.jules/`) are excluded from deployment workflows to save runner resources and reduce deployment noise.
