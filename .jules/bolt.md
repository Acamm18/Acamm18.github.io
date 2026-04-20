## 2026-04-20 - Optimizing CI/CD triggers for journal-only updates
**Learning:** In repositories without application source code, such as those only containing configuration and agent journals, CI/CD pipeline efficiency is the primary performance lever. Preventing redundant deployments triggered by journal updates saves runner resources and reduces deployment noise.
**Action:** Always inspect deployment workflows for opportunities to implement path filters (e.g., `paths-ignore`) for non-production assets like documentation or agent logs.
