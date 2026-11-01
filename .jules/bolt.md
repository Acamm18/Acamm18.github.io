## 2026-11-01 - CI/CD Optimization via Paths Ignore
**Learning:** In repositories primarily containing workflow configurations and agent metadata, updates to internal journal files trigger unnecessary static site deployments. Configuring `paths-ignore: [".jules/**"]` under the push event prevents redundant Action runs and conserves runner resources without impacting production deployments.
**Action:** Always check if workflow triggers can exclude non-production assets and metadata directories like `.jules/**`.
