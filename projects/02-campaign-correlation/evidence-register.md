# Evidence Register

All entries below are fictional and created for this portfolio exercise.

| ID | Observation | Source | Supports | Limitations |
|---|---|---|---|---|
| E-01 | Case A endpoint alert records PowerShell launched by a user-writable script | Simulated endpoint alert excerpt | Suspicious execution hypothesis | No full command line, script, or process tree |
| E-02 | Case A DNS telemetry records `sync-check[.]test` | Simulated DNS log excerpt | Potential link between endpoint activity and hostname | DNS lookup alone does not prove an HTTPS session or maliciousness |
| E-03 | Case B proxy log records HTTPS to `sync-check[.]test` | Simulated proxy log excerpt | Cases A and B may be related | No request path, response, payload, or endpoint process data |
| E-04 | Case C report describes an encoded PowerShell command pattern | Simulated endpoint alert excerpt | Possible behavioral similarity | Pattern is generic and not sufficiently detailed to establish a match |
| E-05 | Events are dated 10–19 March 2026 | Simulated report metadata | Temporal proximity | Time zones and clock accuracy are not verified |

## Evidence-handling notes

- These are scenario statements, not original artifacts.
- No file hashes, packet captures, raw event records, or malware samples are available.
- The evidence is not independently validated.
- Do not describe a scenario statement as a verified real-world indicator.
