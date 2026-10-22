# TLS (Transport Layer Security)

TLS is a cryptographic protocol that provides secure communication over a network.

HTTPS uses TLS to protect HTTP communication by providing confidentiality, integrity, and authentication. SSL is the older predecessor to TLS and is now obsolete.

- **Public-key cryptography:** Used for authentication and key establishment.
- **Symmetric cryptography:** Used for efficient protection of application data.

## TLS Handshake

### Step 1 — ClientHello

The client initiates the TLS handshake by sending the TLS versions and cryptographic options it supports. It may also include supported cipher suites, extensions, and key-share information.

### Step 2 — ServerHello

The server responds with the TLS version and cryptographic parameters it selects. In TLS 1.3, the server also provides key-share information to help establish shared secrets.

### Step 3 — Server Authentication

The server sends its digital certificate in a separate handshake message.

The client verifies the certificate to help establish that the public key belongs to the intended server identity. Verification includes checking the certificate chain, hostname, validity period, and other applicable requirements.

In TLS 1.3, the server also uses a **CertificateVerify** message containing a digital signature to prove possession of the certificate's private key and authenticate the handshake.

### Step 4 — Establishing Secure Communication

The client and server derive shared traffic keys using the handshake's key-establishment process. They then complete the handshake and use symmetric cryptography to protect application data.

## TLS 1.2 vs TLS 1.3

| Feature | TLS 1.2 | TLS 1.3 |
|---|---|---|
| Handshake | Can require more round trips | Usually requires fewer round trips |
| Cipher suites | Supports a wider range of legacy options | Removes many legacy algorithms and options |
| Key exchange | Supports both older and modern methods, depending on the cipher suite | Supports ephemeral (EC)DHE and PSK-based key-establishment modes |
| Forward secrecy | Depends on the negotiated key-exchange method | Provided by ephemeral key exchange; PSK-only modes have different properties |
| 0-RTT | Not supported | Available during certain session resumptions, but early data can be replayed |

**Important security note:** TLS 1.3's 0-RTT early data can be replayed. Applications should avoid using it for operations where replay could cause harm, such as certain financial transactions.

