# Events, Alerts, and Incidents

## 1. Event

- An event is any recorded activity in a system or network.
- An event is not necessarily malicious; it can represent normal or suspicious activity.

**Example:**

| Field | Value |
|---|---|
| User | XXX |
| Action | Login failed |
| Time | 14:32 |
| Source IP | 192.168.X.XX |

## 2. Alert

- An alert is generated when a security detection rule identifies suspicious or potentially malicious behavior.
- An alert requires investigation to determine whether the activity is legitimate or malicious.

**Example:**

47 failed login attempts against user `ved` within 60 seconds.

## 3. Incident

- A security incident is a confirmed or suspected security event that requires investigation or response because it may involve a security compromise.

**Example:**

```text
47 failed login attempts
          ↓
Successful login
          ↓
Unusual source IP
          ↓
Suspicious PowerShell execution
          ↓
Suspicious external connection
          ↓
Potential Security Incident
```

## Relationship Between Events, Alerts, and Incidents

```text
Event → Detection Rule → Alert → Investigation → Incident (if confirmed or suspected)
```

**Important:** Not every event generates an alert, and not every alert becomes an incident. SOC analysts investigate alerts and determine whether an incident needs to be declared.
