## 2026-07-14 - CI/CD Efficiency via Path Exclusions
**Learning:** In repositories primarily consisting of CI/CD workflows and non-production assets (like agent journals), deployments can be triggered unnecessarily by meta-updates.
**Action:** Use 'paths-ignore' in GitHub Action workflows to exclude non-production directories (e.g., '.jules/**') from triggering deployments, saving runner resources and reducing queue noise.
