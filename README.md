# OpportunityRadar

**Version: v0.1.1** — local-first opportunity monitoring dashboard.

## Run
Requires Go 1.22 or later:

```powershell
go run ./cmd/opportunityradar
```

Open `http://127.0.0.1:14236` on the same computer. To build a Windows executable:

```powershell
go build -o OpportunityRadar.exe ./cmd/opportunityradar
```

The application serves a dark dashboard and `GET /api/status`. A scheduler refreshes its state every 30 seconds, saved atomically to `data/state.json`. Four independent radar module slots exist, but **no live source connectors or opportunities are implemented yet**. No fake profit or simulated results are presented as real.

This version uses **standard-library JSON persistence**, not SQLite, React, or Wails. Those are still planned, and are not claimed as delivered. It does not incur paid API/server costs and listens on loopback only.

See `docs/DEVELOPMENT_RULES.md`, `docs/ARCHITECTURE.md`, and `docs/VERSION_HISTORY.md`.
