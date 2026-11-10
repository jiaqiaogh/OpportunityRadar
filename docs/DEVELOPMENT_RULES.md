# Development Rules

1. Canonical repository: `jiaqiaogh/OpportunityRadar`; development branch: `main` only.
2. Read existing repository documentation and source before any change. Never cross-version edit or modify unrelated modules.
3. Reuse existing module entry points; do not create parallel data/decision paths. UI renders only, analysis belongs to backend.
4. Every change requires a real Git commit, incremented `VERSION`, updated `CHANGELOG.md` and `docs/VERSION_HISTORY.md`, with diff and verifiable hashes. Never claim a commit that was not made.
5. No paid servers, paid APIs, or cloud dependencies without explicit approval.
6. No real trading, purchasing, bidding, or unsolicited messaging without explicit approval.
7. Use documented official/free sources; respect rate limits, site terms and applicable law.
8. Do not commit credentials, personal data, or private keys.
9. Keep modules isolated: products, government, business, finance; shared ingestion -> normalization -> analysis -> scoring -> display.
10. Test and report limitations before declaring a version operational.
