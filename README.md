# 🦈 Task 5: Capture and Analyze Network Traffic Using Wireshark  
> 📡 Capturing live network packets, identifying protocols, and analyzing traffic patterns.

---

## 🎯 Objective  
Capture live network packets, identify common protocols, and export them for deeper analysis.

---

## 🛠 Tools Used  
- 🦈 **Wireshark** (Free & Open Source)

---

## 📋 Steps Performed  
1️⃣ Installed and launched **Wireshark**  
2️⃣ Selected Wi-Fi / active network interface  
3️⃣ Generated traffic: 🌐 visited HTTP/HTTPS sites + 📡 ran `ping`  
4️⃣ ⏹ Stopped recording after ~1 minute  
5️⃣ 🔍 Applied filters: `dns`, `tcp`, `http`  
6️⃣ 🧠 Identified observed protocols  
7️⃣ 📤 Exported the `.pcap` file for analysis  

---

## 📡 Protocols Observed  
- 🌍 **HTTP** – Cleartext web traffic (unencrypted)  
- 🔒 **HTTPS** – Encrypted communications via TLS  
- 📦 **TCP** – Reliable, ordered data transfer  
- ❓ **DNS** – Hostname resolutions (hostname ↔ IP)

---

## 🔍 Traffic Insights  
- 📤 Outgoing DNS queries to public servers (e.g., `8.8.8.8`)  
- 🏠 Local IPs masked (`192.168.x.xxx`) for safety  
- 📑 DNS lookups precede HTTP/HTTPS connections

---

## 📂 Files Included  
- 📁 `network_capture.pcap` – Packet capture file  
- 📝 `report.md` – Detailed protocol breakdown

---

## 🚀 How to Use  
1️⃣ Clone or download the repo  
2️⃣ 🦈 Open `.pcap` in Wireshark to explore captured packets  
3️⃣ 📖 Read `report.md` for analysis and insights  

---

## 🔐 Privacy Note  
All internal IP addresses have been safely masked. Public addresses retained for clarity.

---

✅ **Task completed successfully** 🎉

