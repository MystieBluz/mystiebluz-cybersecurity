# 🏡 Home Network Security Hardening

## 📌 Objective  
Assess and improve the security of my home Wi-Fi network. The goal was to **identify vulnerabilities**, apply fixes, and validate improvements.  

---

## 🛠️ Methodology  
1. **Network Mapping:**  
   - Ran `nmap -sn 192.168.1.0/24` to discover devices.  
   - Identified open ports and services on each device.  

2. **Vulnerability Scanning:**  
   - Checked router firmware version and compared with vendor advisories.  
   - Looked for weak/default credentials on IoT devices.  

3. **Remediation Steps:**  
   - Upgraded Wi-Fi encryption to **WPA3**.  
   - Disabled WPS and UPnP.  
   - Updated router firmware.  
   - Enabled firewall & restricted inbound traffic.  

4. **Validation:**  
   - Re-scanned with Nmap to confirm reduced attack surface.  

---

## 📊 Findings  
- Before: Multiple unnecessary open ports (e.g., Telnet, FTP).  
- After: Only HTTPS and DNS traffic remained open.  
- IoT devices required firmware updates.  

---

## 📈 Results  
- Reduced attack surface by ~70%.  
- Strengthened Wi-Fi security with WPA3.  
- Increased awareness of IoT device risks.  

---

## 📸 Screenshots  
![Network Scan Before](./screenshots/before-scan.png)  
![Network Scan After](./screenshots/after-scan.png)  
![Network Diagram](./screenshots/network-diagram.png)  

---

## ✅ Key Takeaways  
- Home networks are **low-hanging fruit** for attackers.  
- Regular scanning and patching are essential.  
- Many IoT devices have poor default security — must be locked down.  
