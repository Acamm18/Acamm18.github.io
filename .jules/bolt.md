## 2026-06-23 - CI/CD Optimization for Journal-Heavy Repos
**Learning:** In repositories primarily used for agent journaling or where meta-files change frequently without affecting the production build, CI/CD triggers should be scoped to ignore these paths to save runner resources.
**Action:** Always check for high-frequency, non-production directories (like .jules/) and add them to paths-ignore in deployment workflows.
