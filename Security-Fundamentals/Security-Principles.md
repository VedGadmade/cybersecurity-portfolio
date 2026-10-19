# Least Privilege

- **Principle:** Give users and processes only the permissions they need to perform their tasks, nothing more.
- **Why?** If an account gets compromised, an attacker may inherit its privileges.
- It minimizes unnecessary access and reduces the potential impact of a compromised account.

# Defense in Depth

- Never rely on a single security control; instead, use multiple layers of security.
- The failure of one control does not necessarily result in a successful compromise.
- **Examples:** Firewalls, IDS/IPS, MFA, endpoint protection, encryption, and access controls.

# Zero Trust

- Zero Trust is a security model based on the principle of **"Never trust, always verify."**
- Access is not automatically trusted just because a user or device is inside the network.
- Every access request is evaluated based on identity, device security, context, and applicable policies.
- **Key principles:**
  - Verify explicitly.
  - Apply least-privilege access.
  - Assume a breach.
- **Examples:** MFA, conditional access, device compliance checks, and network segmentation.
