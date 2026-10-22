# Credential Attacks

### 1. Brute-Force Attack

An attacker repeatedly tries different passwords against a targeted account until they gain access.

- **Pattern:** Many passwords against one account.

### 2. Password Spraying

An attacker tries a small number of commonly used passwords against many accounts.

- **Why?** Repeatedly targeting one account can trigger account lockouts or security alerts.

### 3. Credential Stuffing

An attacker uses previously stolen username-password combinations to attempt access to other services.

- **Why it works:** Users sometimes reuse passwords across multiple services.

### 4. Credential Sniffing

An attacker captures authentication credentials by monitoring network traffic, particularly when insecure protocols or improperly protected communications are used.

### 5. Credential Dumping

An attacker extracts stored credentials, password hashes, or authentication material from a compromised system.

---

# Phishing and Social Engineering

Social engineering uses psychological manipulation or deception to trick people into revealing information, performing actions, or granting access.

### 1. Phishing

Phishing is a social engineering attack in which an attacker deceives a victim into taking an action, such as clicking a malicious link, opening an attachment, or revealing credentials.

### 2. Spear Phishing

A targeted phishing attack directed at a specific individual or organization, often using personalized information to make the message more convincing.

### 3. Whaling

A type of spear phishing that specifically targets high-profile individuals, such as executives or senior management.

---

# Malware

### 1. Virus

Malicious code that attaches itself to a legitimate file or program and typically spreads when the infected file or program is executed.

### 2. Worm

Self-replicating malware that can spread between systems, often across networks, without requiring a user to execute an infected host file on every target.

### 3. Trojan

Malware that disguises itself as legitimate software to trick users into installing or executing it.

### 4. Ransomware

Malware that encrypts files or otherwise prevents access to systems and demands a ransom. Some ransomware operations also steal data before encryption.

### 5. Spyware

Malicious software that secretly collects information about a user's activities or system.

### 6. Rootkit

Malware designed to maintain privileged access and conceal malicious activity or components from users and security tools.

---

# Network and Application Attacks

### 1. DoS (Denial of Service)

An attack that attempts to make a service unavailable to legitimate users by overwhelming or exhausting its resources.

### 2. DDoS (Distributed Denial of Service)

A DoS attack carried out using multiple systems, often compromised devices, to overwhelm a target.

### 3. MITM (Man-in-the-Middle)

An attack in which an attacker positions themselves between two communicating parties to intercept and potentially manipulate their communication.

### 4. SQL Injection (SQLi)

An attack in which malicious SQL input manipulates an application's database queries, potentially allowing unauthorized access to or modification of data.

### 5. Cross-Site Scripting (XSS)

A web application vulnerability that allows attacker-controlled scripts to execute in a victim's browser when they view affected content.

---

# Zero-Day Attack

A **zero-day vulnerability** is a software or system weakness that is unknown to the vendor or for which no effective fix is available.

A **zero-day attack** exploits such a vulnerability before an effective fix is available.

---

# Insider Threat

An insider threat involves a person with authorized access who misuses that access, intentionally or unintentionally, in a way that could harm an organization.

---

# Privilege Escalation

Privilege escalation occurs when an attacker gains permissions beyond those they are authorized to have.

### 1. Vertical Privilege Escalation

A low-privileged user or process gains higher privileges, such as administrator or root access.

**Example:** A standard user gains administrator privileges.

### 2. Horizontal Privilege Escalation

A user gains access to another user's data or resources at a similar privilege level.

**Example:** One standard user accesses another standard user's account data without authorization.

---

# Command and Control (C2)

Command and Control (C2) is the communication mechanism an attacker uses to interact with compromised systems, issue commands, receive information, and maintain control over a compromised environment.

---

# Data Exfiltration

Data exfiltration is the unauthorized transfer of data from an organization's environment to an external or otherwise unauthorized destination.

---

# Drive-by Download

A drive-by download occurs when visiting a compromised or malicious website causes unwanted software to be downloaded or exploits a browser or application vulnerability. Some attacks require user interaction, while others can occur without it.
