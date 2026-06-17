
## 2026-06-17 - Optimizing CI/CD for Asset-less Repositories
**Learning:** In repositories containing only configuration and agent journals, CI/CD efficiency is the primary performance lever. Avoiding redundant deployments by ignoring journal file updates significantly reduces runner usage.
**Action:** Always check for high-frequency, non-production file updates (like agent journals) and exclude them from deployment triggers using `paths-ignore`.
