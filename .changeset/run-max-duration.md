---
"e2e": minor
---

`e2e run --max-duration <ms>` and the config key `maxDuration` stop a run once it has spent that long running tests: nothing more is dispatched, the running tests end as `interrupted`, the rest are skipped with the new cause `time-limit`, and the run records a `RUN_TIMEOUT` error and exits 1. `--last-failed` runs the interrupted and skipped tests next. The report schema's skip causes gain `time-limit`.
