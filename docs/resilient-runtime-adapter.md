# Resilient Runtime Adapter

This repository should not embed a duplicate copy of the resilient runtime engine.

The authoritative runtime lives in `quantam101/already-here-dashboard` and is exposed through:

```text
/api/resilient-runtime
```

## Use cases for this repo

- Lab evidence validation.
- Replay and debrief quality checks.
- Offline-first rubric validation.
- Operator report preflight checks.
- Curriculum data quality checks.

## Adapter contract

Use a thin HTTP client to call:

```text
GET  /api/resilient-runtime/health
POST /api/resilient-runtime/execute
GET  /api/resilient-runtime/events
```

## Required environment variable

```text
ALREADY_HERE_DASHBOARD_URL=https://app.alreadyherellc.com
```

For local development:

```text
ALREADY_HERE_DASHBOARD_URL=http://127.0.0.1:8000
```

## Example validation payload

```json
{
  "query": "validate score not null and score range 0 to 100 then describe",
  "records": [
    {"learner": "operator-001", "score": 92, "track": "soc-tier-1"}
  ],
  "schema_context": {"score": "number", "track": "str"},
  "session_id": "lifelong-catch-correct"
}
```

## Boundary

Do not execute generated Python in this repo. Send declarative validation jobs to the dashboard runtime or use a local deterministic adapter with the same operation allow-list.
