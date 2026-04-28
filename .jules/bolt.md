## 2026-04-28 - Optimizing Journal-Only Repositories
**Learning:** In repositories where the primary activity is documentation or journaling (like agent logs), every update triggers a full CI/CD deployment unless explicitly ignored. This leads to significant resource waste.
**Action:** Always check for `paths-ignore` or equivalent CI filters in repositories that house high-frequency logging or documentation directories.
