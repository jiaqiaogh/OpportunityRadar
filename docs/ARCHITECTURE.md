# Architecture — v0.1.1

## Implemented
- Go standard-library HTTP server (`cmd/opportunityradar/main.go`) on loopback `127.0.0.1:14236`.
- Read-only `GET /api/status` endpoint; HTML dashboard at `/`.
- Four module descriptors: products, government, business, finance; all explicitly marked `awaiting_source`.
- Background 30-second scheduler persists snapshots to `data/state.json` using a temporary file and rename.
- No credentials, real-money actions, or external requests.

## Planned, not implemented
- Official/free API source adapters and rate limiting.
- Shared ingestion -> normalization -> analysis -> scoring -> UI pipeline.
- SQLite migration; React/TypeScript UI and Wails Windows desktop packaging.

This release intentionally delivers a dependency-free, runnable foundation before introducing external build dependencies. It must not be represented as a working market scanner.
