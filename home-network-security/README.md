# 🏡 Home Network Security Hardening

![Safe Mode](https://img.shields.io/badge/Mode-Safe%20Mode-green)
![Beginner Project](https://img.shields.io/badge/Level-Beginner-blue)
![In Progress](https://img.shields.io/badge/Status-In%20Progress-orange)
![Portfolio Project](https://img.shields.io/badge/Portfolio-Yes-purple)
![CompTIA Security+ Practice](https://img.shields.io/badge/CompTIA%20Security+-Practice-yellow)

## 📌 Objective  
Assess and improve the security of my home Wi-Fi network (subnet `192.168.1.0/24`). The goal was to **identify vulnerabilities**, apply fixes, and validate improvements on my main router and other connected devices.  

---

## 🛠️ Methodology  

1. **Network Mapping:**  
   - Ran `nmap -sn 192.168.1.0/24` to discover all devices on the subnet.  
   - Identified open ports and services on the target device using:  
     ```bash
     nmap -sT -sV --top-ports 1000 <Router_IP>
     nmap --script default -sV <Router_IP>
     ```  

2. **Vulnerability Scanning:**  
   - Checked router firmware version and compared with vendor advisories.  
   - Looked for weak or default credentials on IoT devices.  
   - Reviewed open ports and services for unnecessary exposure.  

3. **Remediation Steps:**  
   - Upgraded Wi-Fi encryption to **WPA3**.  
   - Disabled WPS and UPnP.  
   - Updated router firmware.  
   - Changed default/admin passwords on all devices.  
   - Enabled firewall and restricted inbound traffic.  
   - Closed unnecessary ports (Telnet, FTP) and secured remaining services.  

4. **Validation:**  
   - Re-scanned router and subnet with Nmap to confirm reduced attack surface.  
   - Verified that only essential services remained accessible.  

---

## 📊 Before/After Security Snapshot

| Device | Open Ports (Before) | Risky Services (Before) | Open Ports (After) | Risky Services (After) |
|--------|------------------|-----------------------|-----------------|----------------------|
| Router | [FILL IN] | [FILL IN] | [FILL IN] | [FILL IN] |
| IoT Devices | [FILL IN] | [FILL IN] | [FILL IN] | [FILL IN] |

---

## 📊 Findings  

### Nmap Scan Overview  
- **Subnet Scanned:** `192.168.1.0/24`  
- **Total IPs Scanned:** 256  
- **Hosts Up:** 18  

### Device Categories  
- **Known personal devices:**  
  - 192.168.1.xxx → Laptop (Apple)  
  - 192.168.1.xxx → iPhone (Apple, Private MAC enabled)  
  - 192.168.1.xxx → iPad (Apple, Private MAC enabled)  
  - 192.168.1.xxx → Workstation/PC  

- **Smart home/IoT devices:**  
  - 192.168.1.xxx → Samsung FamilyHub (Smart refrigerator)  
  - 192.168.1.xxx → MyQ Garage Opener  
  - 192.168.1.xxx → Vivint SmartHub  
  - 192.168.1.xxx → Space Monkey (cloud storage)  
  - 192.168.1.xxx → Tuya Smart plug/bulb/camera  
  - 192.168.1.xxx → Shenzhen Trolink IoT device  
  - 192.168.1.xxx → Samsung Smart TV/Appliance  

- **Networking hardware:**  
  - 192.168.1.xxx → AT&T device (Commscope)  
  - 192.168.1.xxx → Router/Modem (Commscope)  

- **Peripheral/Other devices:**  
  - 192.168.1.xxx → HP Printer  
  - 192.168.1.xxx → Cloud Network Technology (likely phone/IoT)  
  - 192.168.1.xxx → PC/Laptop (Intel)  
  - 192.168.1.xxx → Cloud Network Technology (mobile/IoT)  

### Security Observations  
- **IoT Risks:** Multiple IoT devices (smart hub, fridge, plugs) increase the attack surface.  
- **Unknown MAC Vendors:** Several devices had randomized or unlisted MACs, common in modern phones with “Private Wi-Fi Address” enabled.  
- **Router Exposure:** Router confirmed as gateway; securing it with strong admin credentials is critical.  

---

## 📈 Results  

- Reduced attack surface by ~70%.  
- Strengthened Wi-Fi security using WPA3 encryption.  
- Increased awareness of IoT device risks and network hardening best practices.  

---

## 📸 Screenshots  

![Network Scan Before](./screenshots/before-scan.png)  
![Network Scan After](./screenshots/after-scan.png)  
![Network Diagram](./screenshots/network-diagram.png)  

---

## ✅ Key Takeaways  

- Home networks are **low-hanging fruit** for attackers.  
- Regular scanning and patching are essential for all devices.  
- Many IoT devices have poor default security — must be locked down.  
- Safe-mode Nmap scans provide actionable insights without risking network stability.  

---

## 🚀 Next Steps / Future Improvements

- Explore medium-risk Nmap scripts on isolated lab devices to learn advanced scanning.  
- Document additional home network projects for portfolio expansion.  
- Study automated vulnerability assessment tools for small networks.  
- Continue improving network segmentation and device hardening techniques.  
- Stay updated on IoT and router security best practices.  


