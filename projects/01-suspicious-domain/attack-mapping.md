# MITRE ATT&CK Mapping — CTI-001

**Important:** This is a provisional mapping of the behavior described in a simulated case. ATT&CK mappings should be tied to observed behavior, not inferred solely from a suspicious indicator.

| Observed / reported behavior | Candidate mapping | Confidence | Rationale and caveat |
|---|---|---|---|
| A suspicious PowerShell process reportedly ran | **T1059.001 — Command and Scripting Interpreter: PowerShell** | Low to moderate, pending raw telemetry | The scenario names PowerShell but does not provide the exact command, process lineage or logs. Confirm before treating as established. |
| Workstation connected over HTTPS to an external domain | No confirmed technique from this fact alone | Low / not mapped | A network connection alone does not establish Command and Control. Determine the connection's purpose, protocol behavior, process ownership and surrounding activity. |
| A file was reportedly downloaded | No confirmed execution mapping | Not established | Downloading a file does not prove it executed. The file was not recovered and execution was not established. |

## Mapping standard

1. State the behavior first.
2. Identify the evidence supporting that behavior.
3. Map only when the behavior matches the technique description.
4. Record uncertainty and missing telemetry.
5. Check the current ATT&CK knowledge base before final publication: https://attack.mitre.org/

This project intentionally avoids assigning an actor based on generic TTP overlap.
