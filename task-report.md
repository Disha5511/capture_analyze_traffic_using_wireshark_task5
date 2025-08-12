# 🦈 Task 5: Capture and Analyze Network Traffic Using Wireshark

## 📜 Summary
In this task, network traffic was captured using **Wireshark** to observe real-time communication between the local machine and various network services. The capture revealed multiple protocols such as **DNS**, **HTTP**, **HTTPS**, **TCP**, **UDP**, and **SSDP**, along with details about their sources, destinations, and purposes.  
This analysis highlights how different protocols work together to enable web browsing 🌐, device discovery 🖥️, and secure communications 🔒.

---

## 🎯 Objective
Capture live network packets using Wireshark, analyze them, and identify at least 3 different network protocols observed during typical usage.

---

## 🛠️ Tools Used
- **Wireshark** (Free, open-source network protocol analyzer)
- **Windows 10** (Operating System)
- **Active Network Connection** (Wi-Fi)

---

## 📝 Steps Performed
1. 📥 Installed **Wireshark** on the system.  
2. 📡 Selected the active **Wi-Fi** network interface.  
3. ▶️ Started packet capture and browsed various websites (**HTTPS** & **HTTP**) to generate traffic.  
4. ⏹️ Stopped capture after ~1 minute of activity.  
5. 🔍 Applied protocol filters like `dns`, `http`, `tcp`, `udp` to isolate packets.  
6. 🧩 Identified multiple protocols from the captured traffic.  
7. 💾 Saved capture as `.pcap` file.  
8. 🖊️ Prepared this analysis report.

---

## 📊 Identified Packets

| Protocol | No. of Packets | Purpose |
|----------|---------------:|---------|
| **DNS** 🌎 | 35 | Resolves domain names to IP addresses. |
| **HTTP** 📄 | 12 | Transfers unencrypted web data. |
| **HTTPS** 🔒 | 54 | Secure, encrypted communication over TLS. |
| **TCP** 📦 | 80 | Reliable data transmission protocol. |
| **UDP** 🚀 | 15 | Lightweight, connectionless data transfer. |
| **SSDP** 📡 | 8 | Used for device discovery on local network. |

---

## 📂 Protocols Identified (Examples from Capture)

| Protocol | Purpose | Example Packet Details |
|----------|---------|------------------------|
| **DNS** 🌎 | Resolves domain names to IP addresses. | Src: `192.168.1.xxx`, Dst: `8.8.8.8`, Query: `www.google.com` |
| **HTTP** 📄 | Transfers unencrypted web data. | Src: `192.168.1.xxx`, Dst: `142.250.183.238`, Method: `GET` |
| **HTTPS** 🔒 | Secure, encrypted communication over TLS. | Src: `192.168.1.xxx`, Dst: `172.217.166.206`, Info: `Client Hello` |
| **TCP** 📦 | Reliable data transmission protocol. | Src: `192.168.1.xxx`, Dst: `142.250.183.238`, Flags: `SYN, ACK` |
| **UDP** 🚀 | Lightweight, connectionless data transfer. | Src: `192.168.1.xxx`, Dst: `224.0.0.251`, Service: `mDNS` |
| **SSDP** 📡 | Used for device discovery on local network. | Src: `192.168.1.xxx`, Dst: `239.255.255.250`, Info: `M-SEARCH` |

---

## 🔍 Observations
- Multiple protocols were captured, showing both **local network discovery** (mDNS, SSDP) and **internet-based communication** (DNS, HTTP, HTTPS).
- DNS queries went to both **public servers** (e.g., `8.8.8.8`) and **local services**.
- HTTPS traffic was encrypted — only TLS handshake details were visible.
- HTTP traffic was in **plain text**, showing methods, URLs, and status codes.

---

## ✅ Conclusion
The capture clearly shows the variety of network protocols involved in everyday internet use. Using Wireshark filters made it easy to analyze each protocol separately.  
This hands-on exercise improved understanding of how **data flows** between devices, servers, and services.

---

**📂 Files Submitted:**
- `task5_capture.pcap` — Raw packet capture
- `task5_report.md` — This report
  

