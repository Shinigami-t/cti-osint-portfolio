# Source Reliability and Independence

## Source inventory

| Source | Type | Reliability assessment | Independence assessment |
|---|---|---|---|
| Case A alert excerpt | Simulated endpoint telemetry summary | Potentially useful, but only a short summary is available | Treat as one primary scenario source |
| Case A DNS excerpt | Simulated DNS telemetry summary | Useful for a recorded lookup if authentic; authenticity is assumed only within the exercise | Different telemetry type, but collection provenance is not supplied |
| Case B proxy excerpt | Simulated network telemetry summary | Useful for a recorded connection if authentic; request details are missing | Presented as a separate organization's log, but cannot be independently validated |
| Case C alert excerpt | Simulated endpoint telemetry summary | Limited by absence of command line and process details | Separate case summary, but its underlying data is unavailable |

## Independence matters

Two documents repeating the same claim do not necessarily provide two independent confirmations. Analysts should trace each statement back to its earliest source and check whether later reports copied the original.

In this exercise, the case summaries are supplied separately, but their provenance cannot be verified. Therefore, treat their apparent independence as an assumption of the scenario, not as a real-world fact.

## Confidence language

- **High confidence:** multiple strong, independent sources support the judgment and major alternatives have been addressed.
- **Moderate confidence:** evidence supports the judgment, but important gaps or alternatives remain.
- **Low confidence:** evidence is sparse, indirect, ambiguous, or dependent on unverified assumptions.

These labels describe the analyst's confidence in a judgment, not the reliability of every source.
