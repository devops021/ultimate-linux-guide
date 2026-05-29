
# OSI (Open Systems Interconnection) Model

The OSI Model is a conceptual framework used to understand how data travels from one computer to another over a network.

It consists of **7 layers**, where each layer performs a specific function.

---

# OSI Model Diagram
```
+-------------------+
| 7. Application    |
+-------------------+
| 6. Presentation   |
+-------------------+
| 5. Session        |
+-------------------+
| 4. Transport      |
+-------------------+
| 3. Network        |
+-------------------+
| 2. Data Link      |
+-------------------+
| 1. Physical       |
+-------------------+
```
Data Flow:
Application → Physical → Network Cable → Physical → Application

---

# Layer 7: Application Layer

## Purpose
Provides network services directly to end users.

## Examples
- HTTP
- HTTPS
- FTP
- SMTP
- DNS

## Real-Life Example
When you open a website in Chrome, the browser communicates using HTTP/HTTPS protocols.

---

# Layer 6: Presentation Layer

## Purpose
Responsible for:
- Data Translation
- Encryption
- Compression

## Examples
- SSL/TLS Encryption
- JPEG
- PNG
- ASCII
- UTF-8

## Real-Life Example
When you visit an HTTPS website, encryption happens at this layer.

---

# Layer 5: Session Layer

## Purpose
Creates, manages, and terminates communication sessions.

## Functions
- Session Establishment
- Session Maintenance
- Session Termination

## Real-Life Example
When you log in to Gmail and remain logged in, the session is managed here.

---

# Layer 4: Transport Layer

## Purpose
Ensures reliable data transfer between systems.

## Protocols
- TCP
- UDP

## Responsibilities
- Segmentation
- Flow Control
- Error Recovery
- Port Management

## Real-Life Example

### TCP
Used for:
- Banking
- Email
- File Transfer

### UDP
Used for:
- Video Streaming
- Online Gaming
- VoIP Calls

## PDU
Segment

---

# Layer 3: Network Layer

## Purpose
Responsible for routing packets between networks.

## Protocols
- IP
- ICMP
- OSPF
- RIP

## Devices
- Router

## Responsibilities
- Logical Addressing
- Route Selection
- Packet Forwarding

## Example
When data travels from Chennai to New York, routers determine the path.

## PDU
Packet

---

# Layer 2: Data Link Layer

## Purpose
Provides communication between devices on the same network.

## Protocols
- Ethernet
- PPP
- ARP

## Devices
- Switch

## Responsibilities
- MAC Addressing
- Frame Creation
- Error Detection

## Example
A switch forwards data based on MAC addresses.

## PDU
Frame

---

# Layer 1: Physical Layer

## Purpose
Transmits raw bits over physical media.

## Examples
- Network Cables
- Fiber Optics
- Wireless Signals
- Connectors

## Devices
- Hub
- Repeater
- Cable

## Example
Electrical signals travel through Ethernet cables.

## PDU
Bits

---

# PDU (Protocol Data Unit)
```
| Layer | PDU |
|---------|---------|
| Application | Data |
| Presentation | Data |
| Session | Data |
| Transport | Segment |
| Network | Packet |
| Data Link | Frame |
| Physical | Bits |

---
```
# Device Mapping
```
| Device | OSI Layer |
|----------|-----------|
| Hub | Layer 1 |
| Repeater | Layer 1 |
| Switch | Layer 2 |
| Router | Layer 3 |
| Firewall | Layer 3-7 |
| Load Balancer | Layer 4-7 |

---
```
# Encapsulation Process

When sending data:

Data
↓
Segment
↓
Packet
↓
Frame
↓
Bits

When receiving data:

Bits
↑
Frame
↑
Packet
↑
Segment
↑
Data

This process is called:
- Encapsulation (Sending)
- Decapsulation (Receiving)

---

# Easy Mnemonic

Top to Bottom:

**All People Seem To Need Data Processing**
```
| Layer | Word |
|---------|---------|
| Application | All |
| Presentation | People |
| Session | Seem |
| Transport | To |
| Network | Need |
| Data Link | Data |
| Physical | Processing |
```
Bottom to Top:

**Please Do Not Throw Sausage Pizza Away**
```
| Layer | Word |
|---------|---------|
| Physical | Please |
| Data Link | Do |
| Network | Not |
| Transport | Throw |
| Session | Sausage |
| Presentation | Pizza |
| Application | Away |

---
```
# Interview Questions

## Q1. Difference between TCP and UDP?
```
| TCP | UDP |
|------|------|
| Connection Oriented | Connectionless |
| Reliable | Faster |
| Error Checking | No Error Recovery |
| Banking | Streaming |

---
```
## Q2. At which OSI layer does a Router work?

Answer: Layer 3 (Network Layer)

---

## Q3. At which OSI layer does a Switch work?

Answer: Layer 2 (Data Link Layer)

---

## Q4. Which layer handles encryption?

Answer: Layer 6 (Presentation Layer)

---

## Q5. What is the PDU of Layer 3?

Answer: Packet
