## 2025-03-07 - Prevent repository bloat during validation
**Learning:** Installing dependencies for validation (like `js-yaml` for workflow checks) can lead to accidental inclusion of `node_modules`, `package.json`, and lock files in the commit, which causes significant repository bloat and violates constraints in repositories that don't already have these files.
**Action:** Always verify `git status` before committing and explicitly reset/delete any temporary files or directories (like `node_modules`) created during the validation process.
