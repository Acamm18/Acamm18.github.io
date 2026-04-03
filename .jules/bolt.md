## 2025-04-03 - Optimizing Deployment CI/CD in pure-config repositories
**Learning:** In repositories containing only configuration files or journals (like GitHub Pages sites with no source code), CI/CD pipeline efficiency is the most impactful performance lever. Enabling `cancel-in-progress: true` for atomic deployments (like GitHub Pages) is a safe way to reduce runner minutes.
**Action:** Always check for `cancel-in-progress: true` in deployment workflows where atomic state is preserved, especially when no application source code is available for optimization.
