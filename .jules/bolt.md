# BOLT'S JOURNAL - CRITICAL LEARNINGS ONLY

## 2025-05-09 - CI/CD Optimization for Journal-only Repository
**Learning:** In repositories without application source code, CI/CD pipeline efficiency is the primary performance lever. Frequent updates to agent journals (like this one) trigger redundant GitHub Pages deployments.
**Action:** Use `paths-ignore` in GitHub Actions workflows to exclude non-production assets (like `.jules/**`) from triggering deployments.
