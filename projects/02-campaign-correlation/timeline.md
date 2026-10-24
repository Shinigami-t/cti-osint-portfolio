# Event Timeline

**All times are illustrative scenario dates. Exact times and time zones were not provided.**

| Date | Case | Observed event | Interpretation limit |
|---|---|---|---|
| 10 March 2026 | A — Northwind Clinic | PowerShell activity appears in a simulated endpoint alert | Execution details and intent are unconfirmed |
| 10 March 2026 | A — Northwind Clinic | DNS lookup for `sync-check[.]test` appears in a simulated DNS excerpt | Lookup does not prove a successful connection or C2 |
| 12 March 2026 | B — Cedar Retail | HTTPS connection to `sync-check[.]test` appears in a simulated proxy excerpt | No payload, URL path, or initiating process is supplied |
| 19 March 2026 | C — Bluehaven Services | Similar-looking encoded PowerShell pattern appears in a simulated alert | No unique command or infrastructure overlap is established |

## Timeline caveats

- Dates are scenario metadata, not verified event times.
- The event order does not establish causality.
- Time zones, clock drift, and collection delays are unknown.
