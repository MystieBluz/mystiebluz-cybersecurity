# 📊 Security Log Analysis & SIEM Simulation

## 📌 Objective  
Simulate a Security Information and Event Management (SIEM) workflow by analyzing Windows logs for suspicious activity.  

---

## 🛠️ Methodology  
1. **Data Collection:**  
   - Enabled Windows Event Logging.  
   - Exported Security Logs (Event IDs: 4624, 4625, 4720).  

2. **SIEM Setup:**  
   - Ingested logs into **Splunk Free** (can also use ELK).  
   - Created custom dashboards.  

3. **Detection Rules:**  
   - Monitored failed logins (Event ID 4625).  
   - Created an alert for multiple failures in < 5 minutes (brute force).  
   - Flagged new user creation events (Event ID 4720).  

4. **Simulation:**  
   - Attempted multiple failed logins to test detection.  

---

## 📊 Findings  
- Successfully detected brute-force attempt simulation.  
- Alert triggered when 5 failed logins occurred within 3 minutes.  
- Dashboard highlighted unusual login times (outside 9–5).  

---

## 📈 Results  
- Built 2 actionable alerts.  
- Gained hands-on SIEM experience.  
- Learned correlation between **logs + detection rules = visibility**.  

---

## 📸 Screenshots  
![SIEM Dashboard](./screenshots/siem-dashboard.png)  
![Failed Logins Graph](./screenshots/failed-logins-graph.png)  

---

## ✅ Key Takeaways  
- SIEM tools allow detection that would be impossible manually.  
- Writing detection rules requires knowing **what normal looks like**.  
- Even basic log analysis provides huge security insight.  
