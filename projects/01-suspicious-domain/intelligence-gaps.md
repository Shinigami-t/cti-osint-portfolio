# Intelligence Gaps and Collection Priorities — CTI-001

## Priority 1 — Validate the endpoint event

- Obtain original endpoint detection and response (EDR) alert details or Windows event / process telemetry.
- Record the full PowerShell command line, parent process, user context, start time and child processes.
- Confirm whether the connection was made by the PowerShell process or another process.

## Priority 2 — Determine what was downloaded

- Search endpoint telemetry and file-system records for the destination path, file hash, file size and creation time.
- If a sample exists, analyze it in an isolated, authorized environment.
- Do not execute unknown files on a normal workstation.

## Priority 3 — Validate infrastructure

- In a real case, collect historical DNS and registration data from documented sources.
- Preserve collection time, query parameters and source provenance.
- Check whether IP associations overlap at the relevant time and account for shared hosting or reassignment.

## Priority 4 — Test attribution

- Trace the Actor Raven claim to its original source.
- Seek independently collected technical evidence.
- Compare specific, unusual behaviors rather than generic use of PowerShell or HTTPS.
- Document alternative hypotheses and the evidence that would distinguish them.

## Priority 5 — Update the assessment

Revise confidence only when new evidence changes the balance between the main hypothesis and plausible alternatives.
