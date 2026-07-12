## 2026-07-12 - CI/CD Path Exclusion
**Learning:** Updating agent-specific files like .jules/bolt.md shouldn't trigger production deployments as they don't affect the site content.
**Action:** Always add paths-ignore for non-production assets in CI/CD workflows to save runner resources.
