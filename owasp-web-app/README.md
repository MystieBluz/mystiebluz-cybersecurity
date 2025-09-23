# 🌐 Secure Web Application Walkthrough (OWASP Top 10 Lite)

## 📌 Objective  
Explore common web app vulnerabilities using **OWASP Juice Shop**, demonstrate exploits, and recommend secure coding fixes.  

---

## 🛠️ Methodology  
1. **Setup:**  
   - Deployed OWASP Juice Shop locally.  

2. **Testing Vulnerabilities:**  
   - **SQL Injection:** Bypassed login using `' OR '1'='1`.  
   - **Cross-Site Scripting (XSS):** Injected `<script>alert('XSS')</script>` into feedback form.  
   - **Insecure Direct Object Reference (IDOR):** Accessed another user’s order history by modifying URL.  

3. **Remediation Recommendations:**  
   - SQL Injection → Use parameterized queries.  
   - XSS → Implement input sanitization & output encoding.  
   - IDOR → Enforce access controls on backend.  

---

## 📊 Findings  
- Application was vulnerable to 3+ OWASP Top 10 issues.  
- Each exploit could compromise **data confidentiality & integrity**.  

---

## 📈 Results  
- Documented vulnerabilities with screenshots.  
- Provided **developer-friendly fixes**.  
- Built a reusable testing checklist for future projects.  

---

## 📸 Screenshots  
![SQL Injection Demo](./screenshots/sql-injection-demo.png)  
![XSS Demo](./screenshots/xss-demo.png)  

---

## ✅ Key Takeaways  
- Web apps are highly exposed targets.  
- Secure coding practices (validate input, sanitize output, enforce auth) are critical.  
- Hands-on testing builds empathy for developers **and** defenders.  
