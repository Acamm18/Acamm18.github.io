## 2026-04-08 - Respecting Developer Warnings in CI/CD Config
**Learning:** Even when a performance optimization like `cancel-in-progress: true` seems technically sound for atomic deployments, it should be avoided if explicit developer comments warn against it. Ignoring such warnings can lead to rejection and may overlook subtle production requirements.
**Action:** Always read and respect inline comments in configuration files; prioritize safety and developer intent over aggressive optimization when they conflict.
