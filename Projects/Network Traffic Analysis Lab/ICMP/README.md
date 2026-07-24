# ICMP Analysis

## Objective

Understand how ICMP is used to verify network connectivity and troubleshoot communication between hosts.


## Theory

Internet Control Message Protocol (ICMP) is a Layer 3 protocol used for diagnostics and error reporting. The `ping` command uses ICMP Echo Requests and Echo Replies to determine whether a destination host is reachable.


## Lab Setup

**Operating System:** Windows

**Tool:** Wireshark

**Display Filter:**
- icmp


**Command Used**

bash:
- ping 8.8.8.8

## Packet Analysis

Observed:

- Echo Request (Type 8)
- Echo Reply (Type 0)
- Source and Destination IP addresses
- TTL values
- Request-response communication


## SOC Relevance

ICMP traffic helps analysts investigate:

- Network connectivity issues
- Packet loss
- Host availability
- Potential ICMP reconnaissance activity


## Key Takeaways

- Understood Echo Request and Echo Reply.
- Learned how ICMP verifies connectivity.
- Interpreted ICMP packet fields using Wireshark.