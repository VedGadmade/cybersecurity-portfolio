# Phishing Investigation Lab

Hands-on phishing email investigations written up as SOC-style incident reports. Each case follows the same workflow an L1 analyst uses when a suspicious email is reported: collect evidence, reach a verdict, and recommend containment.

## What this demonstrates

- Reading email headers and interpreting **SPF, DKIM, and DMARC** results, including alignment
- Investigating sender domains (WHOIS age, DNS records) and sending-IP ownership
- Safe link analysis with urlscan.io, including redirect chains
- Building **IOC tables** and mapping to **MITRE ATT&CK** (T1566)
- Writing a verdict with a confidence level, stating what was **not** confirmed, and recommending containment and detections

## Investigation workflow

1. **Read the message.** What does it want, and who does it claim to be?
2. **Check the sender.** Display name vs address, then SPF, DKIM, DMARC.
3. **Check the domain.** WHOIS creation date and DNS records.
4. **Check the link.** Extract the raw URL, scan without visiting, follow the redirect chain.
5. **Assess impact.** Who else received it, and did anyone click? (Described in each report as recommended checks.)
6. **Verdict and response.** Malicious or not, IOCs, containment, detection ideas.

## Cases

| ID | Summary | Verdict | Techniques |
|---|---|---|---|
| [PH-001](reports/PH-001-mychart-reward-lure.md) | MyChart brand impersonation with a reward lure, routed through cloud storage to a newly registered redirector | Malicious | T1566.002, T1583.001 |


## Tools used

Gmail "Show original" (headers) · Kali Linux (`whois`, `dig`) · urlscan.io · VirusTotal · AbuseIPDB

## Author

Ved Gadmade, focused on SOC Analyst roles.
