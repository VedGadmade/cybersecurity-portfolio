# TCP/IP Model
There are 4 layers of TCP/IP Model:

1. Application Layer - This layer is closest to user application. Provides network services: 
    1. DNS
    2. HTTP
    3. HTTPS
    4. FTP
    5. SMTP
    6. SSH
    7. DHCP 
2. Transport Layer - This layer provides end-to-end communication between applications running on different devices. It uses port number to identify correct application. Transport layer mainly produces TCP segment or UDP Datagram.
3. Internet Layer - Responsible for 
    - Logical addressing
    - Routing packets between network
    - Decide next hop router
    - Deliver packets towards destination
4. Network Access Layer - Responsible for 
    - Creating Frames
    - Physical addressing
    - Communicate with next device on the same network
    - Sending bits through cable or radio signals

### Difference in OSI Model and TCP/IP Model

| OSI model | TCP/IP model | Main responsibility |
| --- | --- | --- |
| 7. Application | Application | Network services used by applications |
| 6. Presentation | Application | Data formatting, encryption, compression |
| 5. Session | Application | Session establishment and management |
| 4. Transport | Transport | End-to-end delivery, reliability, ports |
| 3. Network | Internet | IP addressing and routing |
| 2. Data Link | Network Access/Link | Frames, MAC addresses, local delivery |
| 1. Physical | Network Access/Link | Cables, radio signals, and bits |
