# Architecture — v0.1.0

Target: Go backend, local SQLite, React/TypeScript frontend, Windows desktop packaging with Wails (subject to dependency and toolchain verification).

Pipeline: scheduler -> source adapters -> normalization -> analyzer -> risk/scoring -> local storage -> API -> read-only UI.

Modules: products (price comparison), government (procurement), business (public company demand signals), finance (public market and filing alerts). Each adapter is independent; no live adapters have been implemented in v0.1.0.

Planned release gates: v0.2 products; v0.3 procurement; v0.4 business; v0.5 finance; v1.0 integrated ranking. These are targets, not delivered features.
