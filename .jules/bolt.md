## 2026-06-19 - CI/CD Optimization via paths-ignore
**Learning:** In repositories serving as GitHub Pages sites without application source code, CI/CD pipeline efficiency is the primary performance lever. When 'cancel-in-progress: true' is discouraged by developer comments, 'paths-ignore' provides a safe alternative to prevent redundant deployments caused by non-site updates (like agent journals).
**Action:** Prioritize 'paths-ignore' for documentation and internal tool directories to save runner resources without risking deployment atomicity.
