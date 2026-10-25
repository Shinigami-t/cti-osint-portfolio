# CTI / OSINT Portfolio

A collection of documented investigations demonstrating evidence handling, source evaluation, infrastructure analysis, MITRE ATT&CK mapping, and confidence-aware reporting.

> **Transparency note:** Case 01 is a simulated training investigation. All incident details, reports, domain names, timestamps, and relationships in that case are fictional and must not be presented as real threat intelligence.

## Projects

| ID | Project | Status | Type |
|---|---|---|---|
| 01 | Suspicious Domain Investigation | Complete simulated investigation | Simulated CTI case |
| 02 | [Campaign Correlation Investigation](projects/02-campaign-correlation/README.md) | Complete simulated investigation | Simulated CTI case |
| 03 | [Phishing Infrastructure Investigation](projects/03-phishing-infrastructure/README.md) | Complete simulated investigation | Simulated CTI case |
| 04 | Digital Identity / Persona OSINT | Planned | Ethical OSINT case |
| 05 | Image Geolocation Investigation | Planned | Public image / documented source |
| 10 | Full CTI Investigation | Planned | Capstone |

## Project 01 — Suspicious Domain Investigation

**Question:** Does the available evidence establish that a suspicious domain was malicious and associated with a named threat actor?

- [Read the investigation report](projects/01-suspicious-domain/report.md)
- [Review the evidence register](projects/01-suspicious-domain/evidence-register.md)
- [Review source-dependency analysis](projects/01-suspicious-domain/source-analysis.md)
- [Review ATT&CK mapping](projects/01-suspicious-domain/attack-mapping.md)
- [Review the investigation timeline](projects/01-suspicious-domain/timeline.md)
- [Review intelligence gaps and collection priorities](projects/01-suspicious-domain/intelligence-gaps.md)

## Project 02 — Campaign Correlation Investigation

**Question:** Do three fictional security incidents share enough evidence to be assessed as one campaign?

- [Read the campaign correlation report](projects/02-campaign-correlation/report.md)
- [Review the evidence register](projects/02-campaign-correlation/evidence-register.md)
- [Review source reliability and independence](projects/02-campaign-correlation/source-analysis.md)
- [Review provisional ATT&CK mapping](projects/02-campaign-correlation/attack-mapping.md)
- [Review the event timeline](projects/02-campaign-correlation/timeline.md)
- [Review intelligence gaps and collection priorities](projects/02-campaign-correlation/intelligence-gaps.md)

**Assessment:** The incidents may be related, but the evidence is insufficient to confirm a single campaign or attribute activity to a threat actor.

**Transparency note:** This is a simulated training investigation. All incident details, organizations, domains, and events are fictional.

## Project 03 — Phishing Infrastructure Investigation

**Question:** What can be established about a suspected phishing email and its associated infrastructure, and what evidence is still needed to assess exposure?

- [Read the investigation report](projects/03-phishing-infrastructure/analysis/report.md)
- [Review the initial assessment](projects/03-phishing-infrastructure/analysis/initial-assessment.md)
- [Review indicator analysis](projects/03-phishing-infrastructure/analysis/indicator-analysis.md)
- [Review the investigation timeline](projects/03-phishing-infrastructure/analysis/timeline.md)
- [Review the exposure assessment](projects/03-phishing-infrastructure/analysis/exposure-assessment.md)
- [Review evidence requests](projects/03-phishing-infrastructure/analysis/evidence-requests.md)
- [Review the fictional incident brief](projects/03-phishing-infrastructure/evidence/incident-brief.txt)

**Assessment:** The available scenario is consistent with a phishing attempt, but the original email, infrastructure records, and relevant telemetry are unavailable. Actual compromise and attribution have not been established.

**Transparency note:** This is a simulated training investigation. The domain, email, incident details, and events are fictional.
## Method

For each investigation, distinguish:
1. **Observation:** what a source directly reports or what was directly measured.
2. **Inference:** an interpretation supported by observations.
3. **Assessment:** the current judgement and its confidence.
4. **Intelligence gap:** information that would change or strengthen the assessment.

## Contact

Username {Github} -: Shinigami-t
