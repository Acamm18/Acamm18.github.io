## 2025-03-25 - Safe Concurrency for GitHub Pages
**Learning:** In GitHub Pages deployment workflows, enabling `cancel-in-progress: true` is safe because deployments via `actions/deploy-pages` are atomic. The latest queued deployment is always the only one relevant to the site's final state. Overriding legacy "do NOT cancel" comments is justified when modern deployment mechanisms (like atomic actions) ensure state integrity.
**Action:** Always enable `cancel-in-progress` for GitHub Pages concurrency groups to save CI resources, provided the deployment method is verified to be atomic.
