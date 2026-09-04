# Firewall
A firewall is a security solution that monitors and controls incoming and outgoing network traffic based on predefined security rules.

## Types

- **Stateless Firewall:** This type of firewall operates on layer 3 and layer 4 of the OSI model and works solely by filtering the data based on **predetermined rules** without taking note of the state of the previous connections.
- **Stateful Firewall:** This goes beyond the filtering packets by predetermined rules. It also keep **track of source of previous connection** in the state table. Inspects the packets based on the history(layer 3 and 4)
- **Proxy Firewall:** Problem with above firewall that they are unable to **check the contains of the packets.** Proxy firewalls or the application level gateways acts as an intermediary between clients and external servers and operates primarily at Layer 7.(content filtering policies)
- **Next Generation Firewall(NGFW):** More advanced type of firewall operates between layer 3 to 7. Offers deep packet inspection and enhanced security of incoming and outgoing network traffic. May include integrated IPS capabilities to detect and block malicious activity.

## Rules

- Source Address
- Destination Address
- Source Port
- Destination Port
- Protocol
- Action
- Direction

### Types of Action

1. Allow: Particular traffic defined in this rule is permitted.
2. Deny: Particular traffic defined in this rule is not permitted and blocked.
3. Forward: Redirect traffic on the different network segment.

### **Directionality of Rules**

1. Inbound Rules: Meant to apply on incoming traffic.
2. Outbound Rules: Made for outgoing traffic.
3. Forward Rules: Created to forward specific traffic inside the network.

## Windows Defender Firewall

- Windows Defender Firewall is a built-in host-based firewall included with Windows that monitors and controls inbound and outbound network traffic according to configured rules.
