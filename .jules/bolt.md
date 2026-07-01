## 2026-07-01 - Optimization of CI/CD Trigger via paths-ignore
**Learning:** In a journal-heavy repository where updates frequently occur in non-production directories (like '.jules/'), using 'paths-ignore' is a highly effective lever to reduce CI/CD resource waste without impacting deployment integrity.
**Action:** Always audit repository directories for non-production assets and ensure CI/CD triggers are scoped to relevant paths only.
