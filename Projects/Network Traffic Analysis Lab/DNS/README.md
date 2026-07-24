# DNS Analysis

## Objective

Understand how domain names are translated into IP addresses.

## Theory

DNS (Domain Name System) converts human-readable domain names into IP addresses required for communication.

## Lab Setup

Display Filter:
- dns


Command

bash:
- nslookup openai.com


## Packet Analysis

Observed:

- DNS Query
- DNS Response
- A Records
- AAAA Records
- TTL

## SOC Relevance

DNS analysis helps detect:

- DNS tunneling
- Malware beaconing
- Suspicious domain lookups

## Key Takeaways

Learned how applications locate servers before establishing network connections.