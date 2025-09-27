# 📊 Log File Analyzer  

![Beginner Project](https://img.shields.io/badge/Level-Beginner-blue)  
![Portfolio Project](https://img.shields.io/badge/Portfolio-Yes-purple)  

## 📌 Objective  
Detect suspicious activity in system or server logs by parsing failed login attempts and identifying brute-force patterns.  

---  

## 🛠️ Methodology  
1. **Log File Parsing:**  
   - Scanned through `auth.log` or sample log files.  
   - Identified **failed login attempts** and captured source IPs.  

2. **Suspicious Activity Detection:**  
   - Counted repeated failures from the same IP.  
   - Highlighted the top 5 most suspicious IPs.  

3. **Reporting:**  
   - Output a summary of failed attempts and top offenders.  

---  

## 📊 Key Outcomes  
- Detected brute-force attack patterns.  
- Practiced **file parsing, regex, and automation**.  
- Learned how analysts detect anomalies in log data.  

---  

## 🛠️ Tools & Technologies  
- **Python** – File I/O and regex  
- **Log Files** – Sample SSH or web server logs  
- **Counter (collections)** – Count IP frequency  

---  

## ✅ Key Takeaways  
- Logs are the backbone of intrusion detection.  
- Automating log parsing saves analysts significant time.  
- Even simple scripts can reveal real attack patterns.  

---  

## 🚀 Next Steps / Future Improvements  
- Expand to support **Apache/Nginx web logs**.  
- Output results to a **CSV or dashboard**.  
- Integrate with a **SIEM-like visualization tool**.  

---  

## 📸 Screenshots (Optional)  
- Example failed login attempts detected.  
- Top 5 IPs report output.  
