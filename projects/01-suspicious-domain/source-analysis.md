# Source and Dependency Analysis — CTI-001

## Reporting chain

```text
Simulated Blog A ──> Simulated Vendor Report B
       │                      │
       └─ original claim      └─ repeats attribution
```

Report B cites Blog A for the attribution. Therefore, the two reports do not constitute two independent confirmations of the same claim.

## Assessment of sources

| Source | What it contributes | Independence | What to verify |
|---|---|---|---|
| Simulated SOC alert | Reported endpoint timing and connection | Separate evidence stream within the scenario | Original event logs, process command line, network telemetry |
| Simulated Blog A | Domain-to-campaign claim | Underlying sources are unspecified | Original technical evidence and collection method |
| Simulated Vendor Report B | Actor Raven attribution | Dependent on Blog A for this claim | Whether the vendor has additional unpublished or separately cited evidence |
| Simulated background report | General description of Actor Raven's past behavior | Unknown | Whether claims are sourced and whether behaviors are distinctive |

## Analyst note

Source count is not evidence independence. Assess the origin of each claim, whether sources collected evidence independently, the specificity of the evidence, and whether alternative explanations remain plausible.

These source names and claims are fictional and are included only to demonstrate the method.
