## 2026-04-13 - CI/CD Efficiency as a Performance Lever
**Learning:** In repositories without application source code (e.g., pure configuration or journal-only repos), performance optimization shifts from runtime speed to CI/CD pipeline efficiency. Preventing redundant deployments by ignoring non-essential file updates (like agent journals) saves runner resources and reduces deployment noise.
**Action:** When working in minimal repos, audit workflow triggers for `paths-ignore` opportunities to ensure deployments only happen for meaningful changes.
