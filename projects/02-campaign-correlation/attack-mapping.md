# MITRE ATT&CK Mapping (Provisional)

This mapping is deliberately conservative. A behavior should be mapped only when the evidence supports it; a tool name or network connection alone is not enough.

| Candidate technique | Evidence | Status | What would strengthen the mapping |
|---|---|---|---|
| **T1059.001 — PowerShell** | Cases A and C describe PowerShell-related activity | Provisional | Full process command line, event logs, parent process, and script contents |
| **Command and Scripting Interpreter behavior** | PowerShell is a scripting interpreter, but the activity's purpose is unknown | Do not infer a specific sub-technique beyond the available detail | Validate the actual command and execution context |
| **Command and Control** | Cases A and B include a DNS lookup or HTTPS connection to a fictional hostname | Not established | Evidence of adversary-controlled communications, request/response behavior, or other C2-specific context |

## Mapping note

The presence of PowerShell does not prove malicious activity. A DNS lookup or HTTPS connection does not by itself establish command and control. Revisit mappings if primary telemetry becomes available.

Reference: MITRE ATT&CK, official technique pages at https://attack.mitre.org/ (consult the current pages before using this mapping in a real investigation).
