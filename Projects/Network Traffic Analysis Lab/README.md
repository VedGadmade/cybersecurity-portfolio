**What I Built**
Created a home network analysis lab using Wireshark and Nmap to capture, inspect, and analyze network traffic. Investigated normal network communication and identified reconnaissance activity through packet analysis.

**Tools Used**
Wireshark
Nmap
Kali Linux
Windows
VirtualBox

**What I Did**
Captured and analyzed ICMP, ARP, DNS, TCP, HTTP, and TLS traffic using Wireshark.
Inspected TCP three-way handshakes, DNS queries/responses, ARP resolution, and HTTP requests.
Performed Nmap (-sV) scans to identify open ports and running services.
Correlated Nmap scan results with packet captures to verify service discovery.
Documented findings and mapped reconnaissance activity to MITRE ATT&CK T1046 (Network Service Discovery).

**Investigation Summary**
Observed TCP SYN scanning behavior from a single source host targeting multiple ports on the destination system. Verified open services through SYN–SYN/ACK–RST packet sequences and documented the reconnaissance activity with supporting packet evidence.
