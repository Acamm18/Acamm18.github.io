## 2026-06-10 - [CI/CD Optimization for Journal-Heavy Repositories]
**Learning:** In repositories used primarily for agent logging or documentation, frequent updates to non-code directories (like `.jules/`) can trigger redundant and costly CI/CD runs.
**Action:** Always implement `paths-ignore` for metadata or journal directories in deployment workflows to preserve runner resources and reduce build noise.
