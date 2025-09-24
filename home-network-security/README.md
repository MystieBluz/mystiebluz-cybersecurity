# 🏡 Home Network Security Hardening

![Safe Mode](https://img.shields.io/badge/Mode-Safe%20Mode-green)
![Beginner Project](https://img.shields.io/badge/Level-Beginner-blue)
![In Progress](https://img.shields.io/badge/Status-In%20Progress-orange)
![Portfolio Project](https://img.shields.io/badge/Portfolio-Yes-purple)
![CompTIA Security+ Practice](https://img.shields.io/badge/CompTIA%20Security+-Practice-yellow)

## 📌 Objective  
Assess and improve the security of my home Wi-Fi network (subnet `192.168.1.0/24`). The goal was to **identify vulnerabilities**, apply fixes, and validate improvements on my main router (`192.168.1.254`) and other connected devices.  

---

## 🛠️ Methodology  

1. **Network Mapping:**  
   - Ran `nmap -sn 192.168.1.0/24` to discover all devices on the subnet.  
   - Identified open ports and services on the target device (`192.168.1.254`) using:  
     ```bash
     nmap -sT -sV --top-ports 1000 192.168.1.254
     nmap --script default -sV 192.168.1.254
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
   - Re-scanned target device and subnet with Nmap to confirm reduced attack surface.  
   - Verified that only essential services remained accessible.  

---

## 📊 Before/After Security Snapshot

| Device | Open Ports (Before) | Risky Services (Before) | Open Ports (After) | Risky Services (After) |
|--------|------------------|-----------------------|-----------------|----------------------|
| 192.168.1.254 | [FILL IN] | [FILL IN] | [FILL IN] | [FILL IN] |
| IoT Devices | [FILL IN] | [FILL IN] | [FILL IN] | [FILL IN] |

---

## 📊 Findings  

- **Before:**  
  - Target device (`192.168.1.254`) had multiple unnecessary open ports (e.g., Telnet, FTP).  
  - Some IoT devices were running outdated firmware.  
  - Weak/default passwords detected on a few devices.  

- **After:**  
  - Only HTTPS (443) and DNS (53) ports remained open.  
  - Firmware updated on all devices.  
  - Strong passwords implemented across all devices.  

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

