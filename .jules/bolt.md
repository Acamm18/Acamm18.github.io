## 2026-07-16 - Optimize Deployment Triggers
**Learning:** In repositories without application source code, GitHub Actions deployment triggers can be optimized by ignoring agent-specific directories like .jules/** to avoid redundant runner usage and site redeployments.
**Action:** Always check if GitHub Action workflows can be refined with paths-ignore for non-functional or internal meta-files to improve CI/CD efficiency.
