# Task 5: Capture and Analyze Network Traffic Using Wireshark

## Summary
In this task, network traffic was captured using Wireshark to observe real-time communication between the local machine and various network services. The capture revealed multiple protocols such as DNS, HTTP, HTTPS, TCP, UDP, and SSDP, along with details about their sources, destinations, and purposes. The analysis highlights how different protocols work together to enable web browsing, device discovery, and secure communications.

---

## Objective
The objective of this task was to capture live network packets using Wireshark, analyze them, and identify the most common network protocols observed during typical usage.

---

## Tools Used
- **Wireshark** (Free, open-source network protocol analyzer)
- **Windows 10** (Operating System)
- **Active Network Connection** (Wi-Fi)

---

## Steps Performed
1. **Installed Wireshark** on the system.
2. **Selected the active network interface** (Wi-Fi) in Wireshark.
3. **Started packet capture** and browsed various websites to generate traffic (HTTPS & HTTP) and performed DNS lookups.
4. **Stopped capture after ~1 minute** of traffic generation.
5. Applied **protocol filters** such as `dns`, `http`, `tcp`, `udp` to examine packets.
6. **Identified multiple protocols** from the captured traffic.
7. Exported the capture file in `.pcap` format for submission.
8. Prepared this analysis report.

---

## Identified Packets

| Protocol | No. of Packets | Purpose |
|----------|---------------:|---------|
| **DNS**  | 35 | Resolves domain names to IP addresses. |
| **HTTP** | 12 | Transfers unencrypted web data. |
| **HTTPS** | 54 | Secure, encrypted communication over TLS. |
| **TCP** | 80 | Reliable data transmission protocol. |
| **UDP** | 15 | Lightweight, connectionless data transfer. |
| **SSDP** | 8 | Used for device discovery on local network. |

---

## Protocols Identified (Examples from Capture)

| Protocol | Purpose | Example Packet Details |
|----------|---------|------------------------|
| **DNS** (Domain Name System) | Resolves domain names to IP addresses. | Src: `192.168.1.x`, Dst: `8.8.8.8`, Query: `www.google.com` |
| **HTTP** (HyperText Transfer Protocol) | Transfers unencrypted web data. | Src: `192.168.1.x`, Dst: `142.250.xx.xx`, Method: `GET` |
| **HTTPS** (HTTP Secure) | Secure, encrypted communication over TLS. | Src: `192.168.1.x`, Dst: `172.217.xx.xx`, Info: `Client Hello` |
| **TCP** (Transmission Control Protocol) | Reliable data transmission protocol. | Src: `192.168.1.x`, Dst: `142.250.xx.xx`, Flags: `SYN, ACK` |
| **UDP** (User Datagram Protocol) | Lightweight, connectionless data transfer. | Src: `192.168.1.x`, Dst: `224.0.0.2x1`, Service: `mDNS` |
| **SSDP** (Simple Service Discovery Protocol) | Used for device discovery on local network. | Src: `192.168.1.x`, Dst: `239.255.255.25x`, Info: `M-SEARCH` |

---

## Observations
- **Multiple protocols** were captured, showing both local network discovery (mDNS, SSDP) and internet-based communication (DNS, HTTP, HTTPS).
- DNS queries were sent to both public servers (e.g., `8.8.8.8`) and local network services.
- HTTPS traffic was encrypted, with only TLS handshake details visible.
- HTTP traffic was visible in plain text (method, URL path, status codes).

---

## Conclusion
The packet capture successfully demonstrated the presence of different protocols in normal network usage. The use of filters allowed isolation of specific traffic types for easier analysis. This exercise provided hands-on exposure to packet analysis and network communication patterns.

---

**Files Submitted:**
- `task5_capture.pcap` — Wireshark packet capture file
- `task5_report.md` — This report
