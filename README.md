# 📡 Task 5: Capture and Analyze Network Traffic using Wireshark

## 📝 Objective
Capture live network packets, identify basic protocols, and export them for further analysis.

---

## 🔧 Tools Used
- **Wireshark** (Free & Open Source)

---

## 🛠 Steps Performed
1️⃣ Installed and launched **Wireshark**.  
2️⃣ Selected the active network interface for packet capture.  
3️⃣ Generated traffic by browsing websites (HTTP & HTTPS) and using `ping`.  
4️⃣ Stopped capture after ~1 minute.  
5️⃣ Applied filters to view specific protocols: `dns`, `tcp`, `http`.  
6️⃣ Identified multiple protocols in the capture.  
7️⃣ Exported capture as `.pcap` file.

---

## 📊 Summary of Findings
- **Protocols Observed:**  
  - 🌐 **HTTP** – Cleartext web traffic (unencrypted).  
  - 🔒 **HTTPS** – Encrypted web traffic.  
  - 📦 **TCP** – Transmission Control Protocol (reliable data transfer).  
  - ❓ **DNS** – Domain name lookups (hostname ↔ IP address).  

- **Traffic Insights:**  
  - Public IPs (e.g., `8.8.8.8`) belong to Google DNS.  
  - Private IPs (`192.168.x.xxx`) masked for privacy.  
  - DNS queries occur before HTTP/HTTPS connections.

---

## 📂 Files Included
- `network_capture.pcap` – Full packet capture.  
- `report.md` – Detailed analysis.

---

## 🔒 Privacy Note
- All sensitive internal IP addresses have been masked.  
- Public IPs retained for educational authenticity.

---

✅ **Task Completed Successfully**
