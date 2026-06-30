## 2026-06-30 - Optimize deployment trigger by ignoring journal updates
**Learning:** Frequent updates to the agent journal in `.jules/` trigger redundant GitHub Pages deployments, wasting runner resources and time.
**Action:** Use `paths-ignore` in the workflow `push` trigger to exclude non-production assets like `.jules/**` from triggering deployments.
