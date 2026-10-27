### Investigation: Failed Interactive Logon

**Event ID:** 4625  
**Logon Type:** 2 — Interactive  
**Status:** 0xC000006D  
**Sub Status:** 0xC000006A

**Finding:**  
Windows Security logs recorded a failed interactive logon attempt. The status and sub-status codes indicate a logon failure caused by an incorrect password.

**Assessment:**  
The event confirms an authentication failure but does not independently establish malicious activity. Additional events and account context would be needed to determine whether the attempt was part of a broader attack.

**Recommended follow-up:**
1. Review other failed logons involving the same account.
2. Check whether successful logons occurred before or after the failure.
3. Look for repeated failures within a short time window.
4. Escalate for further investigation if the activity is unusual or forms a suspicious pattern.
