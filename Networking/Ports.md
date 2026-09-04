Port	Service	Description
22	SSH	SSH (Secure Shell) is a protocol used for secure remote login and command execution on Linux/Unix systems. It encrypts all communication using cryptographic algorithms, making it much more secure than Telnet.
80	HTTP	HTTP (Hypertext Transfer Protocol) is used for transferring web pages between a client and a web server. It sends data in plain text, so it is not secure.
443	HTTPS	HTTPS (Hypertext Transfer Protocol Secure) is HTTP over SSL/TLS encryption. It protects data from interception and ensures confidentiality, integrity, and authentication.
53	DNS	DNS (Domain Name System) translates domain names (e.g., google.com) into IP addresses. It primarily uses UDP port 53 for queries and TCP port 53 for zone transfers and large responses.
21	FTP	FTP (File Transfer Protocol) is used to transfer files between systems. It is insecure because usernames, passwords, and data are transmitted in plain text. Secure alternatives are SFTP (SSH File Transfer Protocol) and FTPS (FTP over SSL/TLS).
25	SMTP	SMTP (Simple Mail Transfer Protocol) is used to send emails between mail servers and from email clients to mail servers.
3389	RDP	RDP (Remote Desktop Protocol) is used to remotely access Windows computers with a graphical interface.
445	SMB	SMB (Server Message Block) is used for file sharing, printer sharing, and network resource access in Windows environments.
67/68	DHCP	DHCP (Dynamic Host Configuration Protocol) automatically assigns IP addresses and network settings to clients. The server listens on port 67, and clients use port 68.
