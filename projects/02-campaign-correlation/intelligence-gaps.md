# Intelligence Gaps and Collection Plan

## Priority 1 — Validate the observations
- Obtain raw endpoint, DNS, and proxy records for each case.
- Confirm whether each hostname value was observed directly or copied from another source.
- Record source system, collection time, time zone, and relevant event IDs.
- Preserve source files and calculate hashes for integrity tracking.

## Priority 2 — Test the relationship hypothesis
- Compare full PowerShell command lines and script contents.
- Compare parent-child process relationships, user context, and execution timestamps.
- Compare destination IPs, DNS answers, TLS certificate details, URL paths, and request metadata.
- Determine whether infrastructure was shared hosting or plausibly under common control at the time.

## Priority 3 — Evaluate alternatives
- Check for legitimate software, administrative scripts, or common security tools that could explain PowerShell activity.
- Assess whether the same hostname could have been used by unrelated customers or shared infrastructure.
- Determine whether Cases A and B have independent evidence sources.
- Check for clock skew and differences in timestamp normalization.

## Questions still unanswered
1. Did PowerShell execute successfully, and what did it do?
2. Did either endpoint download or execute a payload?
3. Was `sync-check[.]test` controlled by a common operator during both events?
4. Does Case C share a unique artifact with Cases A or B?
5. Are the three events malicious, benign, or mixed?
6. Is there any defensible basis for actor attribution? Currently, no.

## Stop condition

Do not claim a confirmed campaign or assign a threat actor unless new, independently corroborated evidence supports that conclusion.
