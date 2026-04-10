## 2026-04-10 - CI/CD Optimization via Paths Ignore
**Learning:** In repositories primarily used for agent journals or metadata, updates to these files trigger unnecessary deployment workflows. Using `paths-ignore` for `.jules/**` significantly reduces redundant Action runs and saves runner resources.
**Action:** Always check if a repository has non-functional directories (like `.jules/`) and ensure they are excluded from deployment-triggering workflows.
