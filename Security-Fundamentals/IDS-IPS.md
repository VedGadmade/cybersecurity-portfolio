# IDS (Intrusion Detection System)

An IDS monitors network traffic or host activity for suspicious or malicious behavior. It detects potential threats and alerts the security team but does not typically block attacks. An IDS can identify suspicious activity even when it passes through preventive security controls such as firewalls.

## Types of IDS

IDS can be categorized based on **deployment location** and **detection method**.

### 1. Deployment Location

- **Host-Based IDS (HIDS):** Monitors activity on an individual host, such as system logs, file changes, processes, and system activity. Managing HIDS agents across a large number of hosts can be challenging.

- **Network-Based IDS (NIDS):** Monitors network traffic for suspicious activity. It can provide visibility across multiple systems, depending on sensor placement and network configuration.

### 2. Detection Methods

- **Signature-Based IDS:** Detects known threats by matching observed activity against predefined signatures or patterns. It is effective against known attacks but may fail to detect new or modified threats without updated signatures.

- **Anomaly-Based IDS:** Learns or uses a baseline of normal system or network behavior and identifies deviations that may indicate suspicious activity. It can detect previously unknown threats but may generate false positives.

- **Hybrid IDS:** Combines signature-based and anomaly-based detection to leverage the strengths of both approaches.

# IPS (Intrusion Prevention System)

An IPS detects suspicious or malicious activity and can take preventive actions, such as dropping packets, blocking traffic, or terminating connections, according to its rules and configuration.

## IDS vs IPS

| Feature | IDS | IPS |
|---|---|---|
| Full Form | Intrusion Detection System | Intrusion Prevention System |
| Primary Purpose | Detects suspicious activity | Detects and prevents suspicious activity |
| Action | Generates alerts | Can block or drop malicious traffic |
| Deployment | Often monitors traffic passively | Commonly deployed inline |
| False Positives | Can generate unnecessary alerts | Can potentially block legitimate traffic |

