## 2026-07-09 - CI/CD as the primary performance lever
**Learning:** In repositories like this one (Acamm18.github.io) that lack application source code and consist only of configuration and journal files, traditional application performance optimizations (React.memo, database indexing, etc.) are not applicable. CI/CD pipeline efficiency becomes the primary lever for performance improvements.
**Action:** When working in configuration-only or journal-only repositories, prioritize optimizing workflow triggers and resource usage (e.g., using 'paths-ignore' to skip redundant deployments).
