# Bolt's Journal

## 2025-02-17 - Optimizing CI/CD for Static Site
**Learning:** In a minimal GitHub Pages repository, the primary performance bottleneck is unnecessary CI/CD runs and resource wastage from redundant builds.
**Action:** Always enable `cancel-in-progress: true` for deployments where only the final state matters, and use `paths-ignore` for non-functional directories like `.jules/`.
