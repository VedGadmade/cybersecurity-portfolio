# VPN (Virtual Private Network)

A Virtual Private Network (VPN) creates a protected network connection over an underlying network, such as the internet.

## What Does a VPN Provide?

- **Encryption:** Protects data transmitted through the VPN tunnel.
- **Secure Remote Access:** Allows authorized users to access an organization's internal network remotely.
- **Site-to-Site Connectivity:** Connects networks at different office locations securely.
- **Authentication:** Verifies the identity of users or devices connecting to the VPN.

## Types of VPN

### 1. Full Tunnel VPN

Most or all applicable client traffic is routed through the VPN tunnel, depending on the configuration.

- Internet traffic and internal network traffic typically pass through the VPN.
- Allows an organization to apply security monitoring and filtering to routed traffic.
- Can increase bandwidth usage on the organization's network.

### 2. Split Tunnel VPN

Only selected traffic is routed through the VPN tunnel. Other traffic uses the user's regular internet connection.

- Reduces the amount of traffic routed through the organization's network.
- Can improve network performance.
- May introduce security risks if direct internet traffic bypasses organizational security controls.

### 3. Remote Access VPN

Allows individual users to connect securely to an organization's internal network from a remote location.

**Example:** An employee connects to the company network from home using a VPN client.

### 4. Site-to-Site VPN

Creates a secure connection between two or more networks, such as networks belonging to different office locations.

**Example:** A company securely connects its Pune and Mumbai office networks.

