# IP Address and Subnetting
IP address stands for Internet Protocol which is identity of each host. 

There are two types of IP address:

1. **IPv4:** Contains 32 bits which are divided into 4 groups of 8 bits called octets. Each octets can contain 0 - 255
2. **IPv6:** Uses 128 bits which are divided into 8 groups each group contains 4 hexadecimal digits. 

## Public IP Vs Private IP

**Public IP** is used inside the internal network and are not directly routable on the public network

**Private IP** is globally routable on internet and can be assigned to router.

# Subnetting

Subnetting is the process of dividing a large IP network into smaller logical networks called subnets

## Subnet Mask

It tells us which bit belong to the network and which bits belong to the hosts

## CIDR Notation

Classless Inter-Domain Routing - The number represents the number of network bits.

Example - 192.168.1.25/24

24 network bits
8 host bits

## CIDR - Subnet Mask

/24 → 255.255.255.0
/25 → 255.255.255.128
/26 → 255.255.255.192
/27 → 255.255.255.224
/28 → 255.255.255.240
/29 → 255.255.255.248
/30 → 255.255.255.252

## Host per Subnet

Usable Hosts = 2^h - 2

h = number of host bits  

**Why minus 2? -**  Network address and Broadcast address cannot be assigned to normal hosts.

| CIDR | Host Bits | Total Addresses | Usable Hosts |
| --- | --- | --- | --- |
| /24 | 8 | 256 | 254 |
| /25 | 7 | 128 | 126 |
| /26 | 6 | 64 | 62 |
| /27 | 5 | 32 | 30 |
| /28 | 4 | 16 | 14 |
| /29 | 3 | 8 | 6 |
| /30 | 2 | 4 | 2 |
| /31 | 1 | 2 | special point-to-point use |
| /32 | 0 | 1 | single address |

## NAT

Network Address Translation : It allows private address communicate through a public address.
Internal Network

192.168.1.10 ─┐
192.168.1.11 ─┼──> Router/NAT ──> Public IP ──> Internet
192.168.1.12 ─┘
