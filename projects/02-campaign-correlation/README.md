# Project 02 — Campaign Correlation Analysis

**Type:** Simulated CTI case study  
**Status:** Portfolio-ready training exercise  
**Purpose:** Demonstrate how to compare related incident reports without overstating attribution.

## Scenario

Three fictional organizations report suspicious activity during a two-week period. The reports contain overlapping infrastructure and behavioral clues, but the available evidence is incomplete. The analyst must assess whether the incidents are plausibly related, identify what is and is not corroborated, and recommend next collection steps.

**All organizations, domains, IP addresses, timestamps, and reports in this exercise are fictional.** The reserved `.test` domain is used to avoid implicating real infrastructure. This is not a claim about a real threat actor or campaign.

## Files

- [`report.md`](report.md) — executive assessment and analytic reasoning
- [`evidence-register.md`](evidence-register.md) — evidence, limitations, and confidence
- [`source-analysis.md`](source-analysis.md) — source reliability and independence
- [`timeline.md`](timeline.md) — event sequence
- [`intelligence-gaps.md`](intelligence-gaps.md) — unresolved questions and collection plan
- [`attack-mapping.md`](attack-mapping.md) — cautious ATT&CK mapping

## Key analytic rule

**Similarity is not proof of common control.** Shared infrastructure can support a relationship hypothesis, but it can also reflect shared hosting, copied reporting, or unrelated activity. Attribution requires stronger, independently corroborated evidence.

## Suggested GitHub placement

Copy this folder into your existing portfolio repository as:

`projects/02-campaign-correlation/`

Then link it from the main portfolio `README.md`.
