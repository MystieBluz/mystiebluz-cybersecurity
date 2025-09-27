# 🔑 Password Strength Checker  

![Beginner Project](https://img.shields.io/badge/Level-Beginner-blue)  
![Portfolio Project](https://img.shields.io/badge/Portfolio-Yes-purple)  

## 📌 Objective  
Evaluate the security of user-entered passwords and optionally check if they appear in known data breaches. This builds foundational skills in **secure coding practices, regex, and API usage**.  

---  

## 🛠️ Methodology  
1. **Password Strength Rules:**  
   - Checked for length (minimum 8 characters).  
   - Required uppercase, lowercase, numbers, and symbols.  
   - Flagged dictionary words as weak.  

2. **Optional Breach Check:**  
   - Integrated with the **HaveIBeenPwned API** to verify if the password has been exposed in past data breaches.  

3. **Strength Evaluation:**  
   - Rated passwords as **Weak, Moderate, or Strong** based on scoring system.  

---  

## 📊 Key Outcomes  
- Identified weak and reused passwords.  
- Practiced **regex, string handling, and API calls**.  
- Learned how real-world tools like password managers enforce strength rules.  

---  

## 🛠️ Tools & Technologies  
- **Python** – Core scripting language  
- **Regex** – Pattern matching for password rules  
- **Requests Library** – API integration  

---  

## ✅ Key Takeaways  
- Strong, unique passwords are critical to reducing account compromises.  
- Even strong passwords can be unsafe if leaked in data breaches.  
- Automating checks helps enforce security standards.  

---  

## 🚀 Next Steps / Future Improvements  
- Add a **GUI interface** for non-technical users.  
- Implement **password entropy calculation** for more accurate scoring.  
- Expand breach check to batch process multiple passwords.  

---  

## 📸 Screenshots (Optional)  
- Example terminal outputs for weak, moderate, and strong passwords.  
- Screenshot of breach detection result.  
