---
"e2e": minor
---

`E2E_CACHE_DIR` and `e2e run --cache-dir <dir>` (also on `e2e cache`) replace `cache.dir`, so checkouts and worktrees of one project can share a replay cache without editing the config. The flag wins over the variable, both resolve from the project root, and the cache mode stays as configured.
