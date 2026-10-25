# Indicator Analysis — Operation Glass Finch

## Indicator 1: Sender email

- **Value:** it-support@northstar-verify.example
- **Source:** Employee-provided email copy
- **Observation:** The address claims to represent IT support, but the domain does not establish that the sender is affiliated with the organization.
- **Assessment:** Suspicious in context; sender legitimacy has not been independently verified.
- **Limitation:** Original email headers and domain ownership records are unavailable.

## Indicator 2: URL

- **Value:** hxxps://northstar-verify.example/session
- **Source:** Employee-provided email copy
- **Observation:** The link leads to a path named `/session`, and the employee reports seeing a sign-in page.
- **Assessment:** Consistent with a possible credential-harvesting lure when considered alongside the email's suspension threat.
- **Limitation:** The path name alone does not prove malicious functionality. No page capture or server-side evidence is available.

## Indicator 3: Sender display name

- **Value:** Corporate IT Helpdesk
- **Source:** Employee-provided email copy
- **Observation:** The display name presents the sender as an internal support team.
- **Assessment:** Could be used to create trust, but display names can be chosen by senders and do not authenticate identity.
- **Limitation:** The original headers and authentication results are unavailable.

## Overall assessment

The indicators collectively support a preliminary phishing assessment. They do not independently establish credential theft, successful compromise, infrastructure ownership, or threat actor attribution.
