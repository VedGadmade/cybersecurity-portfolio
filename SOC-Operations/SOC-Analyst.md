# What is the work of SOC analyst?
SOC is responsible for monitoring organization’s system and network to: 

- Detect suspicious activity
- Identify threats
- Investigate alerts
- Contain attacks

## Workflow

```
          SECURITY DATA
                ↓
    ┌──────────────────────┐
    │ Logs / Network / EDR │
    └──────────┬───────────┘
               ↓
              SIEM
               ↓
          Detection
               ↓
             ALERT
               ↓
         SOC L1 Analyst
               ↓
      ┌────────┴─────────┐
      ↓                  ↓
   False Positive     Suspicious
                          ↓
                     Investigate
                          ↓
                   Determine Scope
                          ↓
                ┌─────────┴─────────┐
                ↓                   ↓
             Close              Escalate
```
