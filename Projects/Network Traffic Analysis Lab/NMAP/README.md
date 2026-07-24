# Nmap Service Discovery

## Objective

Understand how network reconnaissance identifies open services.

## Theory

Nmap is a network scanning tool used to discover hosts, open ports, and running services.

## Lab Setup

Command

bash:
nmap -sV <target-ip>


## Packet Analysis

Observed:

- TCP SYN packets
- SYN-ACK responses
- RST packets
- Open TCP ports
- Service detection

## MITRE ATT&CK Mapping

**T1046 – Network Service Discovery**

## SOC Relevance

SOC analysts use packet analysis to identify unauthorized reconnaissance and potential attack preparation.

## Key Takeaways

Correlated Nmap scan results with Wireshark captures to verify open services and identify SYN scanning behavior.