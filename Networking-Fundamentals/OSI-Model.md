# OSI Model
OSI (Open System Interconnection)  model is a 7 layer framework which standardize how different networking protocol  and devices communicate.

| Layer | Function | Ports  | Protocol | Devices |
| --- | --- | --- | --- | --- |
| Physical | Converts frames into electrical, optical, or radio signals for transmission over cables or wireless media | N/A | Ethernet cables, Wi-Fi | Hubs, Repeater, Cables, NICs, Modem |
| Data Link | Physical Addressing (MAC). Switches forward frames within network  | N/A | Ethernet, ARP, PPP, STP, VLAN  | Switches, Bridges, NICs |
| Network | Logical Addressing (IP). Routers forward packets between different networks. | N/A | IP (IPv4, IPv6), ICMP, OSPF, IPSec | Routers, Layer 3 switches, Firewall |
| Transport | Provides Reliable or Unreliable delivery. Adds port number to identify which application should receive the data | 1 - 65535 (all ports)  | TCP, UDP, SCTP | Load Balancer, End hosts, Firewall(L4) |
| Session | Manages session between application | Not strictly defined | NetBIOS, RPC, PPTP  | End Hosts, Firewall  |
| Presentation | Translation , encrypts(SSL/TLS)  and compress  | Varies by application |  JEPG, MPEG, ASCII | End Hosts, Gateways |
| Application | Interface between user applications and network; provides network services to end-user applications | 80 - HTTP, 443 - HTTPS, 21 - FTP, 22 - SSH, 25 - SMTP, 53 - DNS,  | HTTP, HTTPS, FTP, SSH, SMTP, DNS | End Hosts(Computers, Servers), Firewalls,  |

### Encapsulation

Layer 7 (Application Layer) - Creates Data (messages)

Layer 6 (Presentation Layer) - Formats, Encrypts or compresses data

Layer 5 (Session Layer) - Adds session information

Layer 4 (Transport Layer) - Adds source port and destination port also creates Segment(TCP) or Datagram(UDP)

Layer 3 (Network Layer) - Adds source IP and destination IP also creates packets

Layer 2 (Data Link Layer) - Adds source/destination MAC address and trailer (CRC) also creates Frame 

Layer 1 (Physical Layer) - Converts the frame into bits for transmission

### Decapsulation

Layer 1 (Physical Layer) - Receive signal and convert them back to bits

Layer 2 (Data Link Layer) - Reads MAC addresses, checks CRC, and removes the frame header/trailer

Layer 3 (Network Layer) - Reads IP address remove IP header passes segment up 

Layer 4 (Transport Layer) - Reads Port No. and remove transport header

Layer 5 (Session Layer) - Reads Session ID

Layer 6 (Presentation Layer) - Decrypts, Decompress or reformat

Layer 7 (Application Layer) - Deliver data to receiving application
