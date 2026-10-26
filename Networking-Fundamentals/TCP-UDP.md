# TCP (Transmission Control Protocol)

- **Uses segments:** Divides application data into segments for transmission.
- **Reliable:** Uses acknowledgements and retransmissions to provide reliable delivery.
- **Connection-oriented:** Establishes a connection before transmitting application data.
- **Retransmits lost segments:** Retransmits data when loss is detected.

## Three-Way Handshake

The TCP three-way handshake establishes a connection between a client and a server.

```text
Client                                      Server
  |                                           |
  | -------- SYN, Seq = x -------------------> |
  | <--- SYN + ACK, Seq = y, Ack = x+1 ------- |
  | -------- ACK, Ack = y+1 -----------------> |
  |                                           |
          Connection Established
```

### Steps

**1. SYN (Synchronize)**

- The client sends a segment with the SYN flag set.
- It provides the client's initial sequence number, `x`.
- It requests to establish a TCP connection.

**2. SYN-ACK (Synchronize-Acknowledge)**

- The server responds with the SYN and ACK flags set.
- It provides its own initial sequence number, `y`.
- `Ack = x + 1` acknowledges the client's SYN.

**3. ACK (Acknowledge)**

- The client sends an ACK segment.
- `Ack = y + 1` acknowledges the server's SYN.
- The TCP connection is established.

## Four-Way Termination

TCP typically uses four segments to terminate a connection gracefully because each direction of communication is closed independently.

### Steps

**1. FIN (Finish)**

- One side sends a segment with the FIN flag set.
- It indicates that it has finished sending data.

**2. ACK (Acknowledge)**

- The other side acknowledges the FIN.
- It may continue sending any remaining data.

**3. FIN (Finish)**

- After finishing its own data transmission, the other side sends a FIN segment.

**4. ACK (Acknowledge)**

- The first side acknowledges the second FIN.
- The TCP connection is closed after the required TCP state transitions.

*Note: TCP termination may use fewer than four segments when acknowledgements and FIN flags are combined. The exact sequence depends on the connection state.*

## Sequence Numbers

TCP treats application data as a **stream of bytes**. Each byte is associated with a sequence number.

- Sequence numbers help TCP track transmitted data.
- Acknowledgement numbers indicate the next byte expected by the receiver.
- TCP uses sequence and acknowledgement numbers to detect missing data and support reliable, ordered delivery.

For example, if a segment starts at sequence number `1000` and carries 500 bytes, the next expected sequence number is `1500`.

---

# UDP (User Datagram Protocol)

- **Uses datagrams:** Sends data in individual datagrams.
- **Connectionless:** Does not establish a connection through a handshake before sending data.
- **Low overhead:** Has a smaller protocol header and avoids TCP's connection-management and retransmission mechanisms.
- **No guaranteed delivery:** Datagrams may be lost or arrive more than once.
- **No guaranteed ordering:** Datagrams may arrive out of order.
- **No built-in retransmission mechanism:** UDP itself does not retransmit lost datagrams.

## Common Uses of UDP

- DNS queries
- Voice over IP (VoIP)
- Live audio and video streaming
- Online gaming
- DHCP

## TCP vs UDP

| Feature | TCP | UDP |
|---|---|---|
| Connection | Connection-oriented | Connectionless |
| Data unit | Segment | Datagram |
| Reliability | Reliable delivery mechanisms | No built-in delivery guarantee |
| Ordering | Provides ordered byte-stream delivery | No built-in ordering guarantee |
| Retransmission | Supports retransmission | No built-in retransmission |
| Overhead | Higher | Lower |
| Common uses | HTTPS, SSH, email | DNS, VoIP, gaming, DHCP |
