## 2026-05-07 - Hidden Directory Awareness
**Learning:** Standard directory listings like `ls -R` fail to reveal this repository's critical content (which resides in hidden directories like `.github` and `.jules`); the root appears empty but it is not.
**Action:** Always use `ls -la` or `find .` to accurately audit the file structure.
