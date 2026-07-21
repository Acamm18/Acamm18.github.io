## 2026-07-21 - Prevent Redundant Deployments on Agent Journal Updates
**Learning:** In purely administrative/journal-based repositories containing only static-content deployment workflows, updates to agent journal files (e.g., .jules/**) trigger redundant, non-production deployments that waste GitHub Actions resources.
**Action:** Configure paths-ignore: [".jules/**"] on the push workflow trigger to explicitly exclude agent journal files from initiating deployment actions, thereby optimizing pipeline efficiency.
