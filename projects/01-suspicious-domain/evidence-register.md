# Evidence Register — CTI-001

All entries below are fictional case material, not observations collected from a real system.

| ID | Reported observation / claim | Source | Type | Limitations |
|---|---|---|---|---|
| E-01 | `WS-104` connected to `northstar-update[.]test/update/check` over HTTPS on 2026-03-14 10:32 UTC | Simulated SOC alert | Reported endpoint observation | Raw logs and packet capture not supplied |
| E-02 | Suspicious PowerShell process ran shortly before the connection | Simulated SOC alert | Reported endpoint observation | Command line, process tree and exact timing not supplied |
| E-03 | Downloaded file was not recovered | Simulated SOC alert | Evidence gap | File content and execution status unknown |
| E-04 | Domain was associated with a malware campaign | Simulated threat blog A | Source claim | Underlying technical evidence not supplied |
| E-05 | Campaign attributed to Actor Raven | Simulated vendor report B | Source claim | Cites blog A; no independent artifact provided |
| E-06 | Actor Raven historically used PowerShell, HTTPS and newly registered domains | Simulated background report | Contextual claim | Broad behaviors are not unique to one actor |
| E-07 | Domain reportedly resolved to multiple IP addresses over time | Simulated DNS notes | Infrastructure claim | No original DNS dataset supplied; timing and provenance require verification |
| E-08 | One IP reportedly hosted unrelated domains at other times | Simulated DNS notes | Infrastructure context | Shared hosting / reassignment may explain overlap |

## Handling rule

Do not upgrade a reported claim into a directly verified fact. In a real investigation, preserve the original source, collection time, query or method, and supporting artifact.
