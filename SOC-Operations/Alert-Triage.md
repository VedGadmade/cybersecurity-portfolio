# Alert Triage

Alert triage is the process of reviewing, categorizing, validating, and prioritizing security alerts to determine which require immediate investigation and which may be false positives.

## Alert Prioritization

Prioritize alerts based on:

- **Severity:** How serious the potential threat is.
- **Business Impact:** Potential damage to business operations or data.
- **Confidence:** How strongly the available evidence supports the detection.
- **Threat Type:** The nature of the suspected attack.
- **Affected Assets:** The importance and sensitivity of the affected systems.
- **Spread:** Whether the activity has affected or could affect additional systems.

## How Do You Determine Severity?

Consider the following factors:

- Business impact
- Affected assets
- Threat type
- Likelihood of a successful attack
- Scope and spread of the activity
- Potential damage if the threat is confirmed

## The 5 Ws of Alert Investigation

| Question | Answer |
|---|---|
| **What?** | A potentially malicious file was detected on a host inside the organization's network. |
| **When?** | The file was detected at 13:20 on June 5, 2024. |
| **Where?** | The file was detected on the host named `GEORGE PC`. The exact file path should also be recorded. |
| **Who?** | The detection was associated with the user George. |
| **Why?** | The investigation found that the file had been downloaded from a website distributing pirated software. During the interview, the user confirmed downloading it to obtain software for free. |

**Important:** A suspicious file or pirated download does not automatically prove that a system is compromised. Verify the file's hash and reputation, detection details, execution status, and related endpoint or network activity before deciding whether the alert is a true positive.

## Next Steps

1. Validate the alert and collect supporting evidence.
2. Determine severity and business impact.
3. Check whether the file was executed and whether other systems are affected.
4. Contain the threat if necessary, following organizational procedures.
5. Document findings and escalate or close the alert with justification.
