## 2026-09-29 - CI/CD Efficiency via Path Exclusions
**Learning:** In repositories containing only deployment workflows and agent journals, internal metadata/documentation updates trigger unnecessary GitHub Actions deployment runs.
**Action:** Always add `paths-ignore: [".jules/**"]` to workflow push triggers when managing internal agent files.
