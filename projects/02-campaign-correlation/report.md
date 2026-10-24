# Campaign Correlation Assessment

## Executive summary

Three fictional incident reports show a limited set of overlapping indicators and behaviors over 10–19 March 2026. The strongest overlap is that two reports independently recorded connections to the same fictional hostname, `sync-check[.]test`. A third report describes a similar PowerShell command pattern but does not include the hostname.

**Assessment:** The incidents may be related, but the evidence is insufficient to conclude that they belong to one campaign.  
**Confidence:** Low to moderate for a possible relationship; low for a single-operator or single-campaign conclusion.  
**Attribution:** Not assessed. No real threat actor is named or implied.

## Scope and assumptions

This is a simulated training case. All organizations, telemetry, domains, dates, and report content are invented. No live indicators were investigated.

The analysis distinguishes:
- **Observation:** directly stated in the fictional evidence.
- **Inference:** an interpretation that could explain the observations.
- **Unknown:** a question the available evidence cannot answer.

## Incident summaries

- **Case A — Northwind Clinic:** Endpoint alert records PowerShell launched by a user-writable script and an outbound DNS lookup for `sync-check[.]test`. The available excerpt does not show the full command line or subsequent process behavior.
- **Case B — Cedar Retail:** Proxy logs record an HTTPS connection to `sync-check[.]test` two days later. No endpoint process telemetry was supplied.
- **Case C — Bluehaven Services:** An endpoint alert records a PowerShell command with a similar encoded-command pattern. The report does not include DNS, proxy, or destination details.

## Evidence correlation matrix

| Comparison | Case A vs. Case B | Case A vs. Case C | Analytical significance |
|---|---|---|---|
| Hostname | Same fictional hostname reported | No hostname supplied for Case C | The A-B overlap warrants follow-up, but shared hostname control is unverified |
| PowerShell behavior | Case B has no endpoint process telemetry | Both reports describe PowerShell-related activity | Similarity is too general to establish a unique technical match |
| Timing | Events are two days apart | Within the overall reporting window | Temporal proximity is context, not proof of a relationship |
| Independent corroboration | Original logs and collection provenance require verification | Full command lines and process evidence are missing | The available summaries are insufficient to establish a common campaign |

The strongest current lead is the shared hostname in Cases A and B. Case C remains a weaker potential association because its reported PowerShell pattern lacks a distinctive, independently verifiable match. No relationship should be treated as confirmed until the underlying evidence is obtained and validated.

## Correlation analysis

### Supporting the relationship hypothesis
1. Cases A and B name the same fictional hostname.
2. Cases A and C describe PowerShell-related activity with a superficially similar pattern.
3. The activity falls within a relatively short time window.

### Limiting the relationship hypothesis
1. The available material does not establish that the hostname was controlled by the same operator during both events.
2. Case B has network evidence only; no process or payload evidence is supplied.
3. The similarity in PowerShell patterns is not sufficiently detailed to establish a unique match.
4. The reports do not include hashes, payload samples, certificate details, DNS history, or independently validated infrastructure ownership.
5. The three incidents may have different causes, or some similarities may be coincidental.

## Competing hypotheses

- **H1 — One related activity cluster:** all three incidents are connected through a common operator or campaign.
- **H2 — Two related incidents plus one coincidental lookalike:** Cases A and B are related; Case C is unrelated.
- **H3 — Superficial overlap:** the incidents are unrelated, and the similarities reflect common tools or infrastructure.

The current evidence supports investigating H1 and H2, but does not reliably distinguish them from H3.

## Judgments

| Judgment | Confidence | Rationale |
|---|---|---|
| Cases A and B warrant correlation follow-up | Moderate | Same hostname appears in two different telemetry types, but provenance and control are unverified |
| Case C belongs to the same cluster | Low | Similar behavior is described without a unique technical match |
| All three cases are one campaign | Low | Key corroborating evidence is absent |
| A specific threat actor is responsible | Not assessed | No reliable attribution evidence |

## Recommended next steps

1. Obtain original, timestamped logs for Cases A and B and confirm that the hostname values were observed directly rather than copied from another report.
2. Collect full PowerShell command lines, parent processes, script contents, and process hashes from Cases A and C.
3. Compare DNS answers, TLS certificate metadata, URL paths, request headers, and hosting history where available.
4. Check whether timestamps use consistent time zones and whether the events fall within the same operational window.
5. Preserve raw evidence and document collection method, source, and hash for each artifact.
6. Update the assessment only when new evidence materially changes the competing hypotheses.

## Limitations

This exercise uses invented summaries rather than raw logs. It cannot establish maliciousness, execution, command-and-control, common operator, or attribution. ATT&CK mappings are provisional and require confirmation from primary telemetry.
