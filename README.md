# 🔐 Security Audit - Internee.pk  

## 📌 Objective  
Conduct a security audit of **Internee.pk’s website** to identify vulnerabilities and ensure data protection.  

---

## 📊 Scope  
- Login & Authentication  
- User Profiles  
- API Endpoints  

---

## 🛠 Tools Used  
- [OWASP ZAP](https://www.zaproxy.org/) – Automated scanning  
- [Burp Suite](https://portswigger.net/burp) – Manual interception & payload testing  
- Manual Penetration Testing  

---

## 🚨 Findings  

### 1️⃣ SQL Injection (High)  
- **Location:** `/login`  
- **Payload:** `' OR '1'='1 --`  
- **Impact:** Authentication bypass  

### 2️⃣ Cross-Site Scripting (XSS) (Medium)  
- **Location:** `/search`  
- **Payload:** `<script>alert('XSS')</script>`  
- **Impact:** Session hijacking risk  

### 3️⃣ Missing Security Headers (Medium)  
- **Location:** All pages  
- **Impact:** Increased attack surface for XSS/Clickjacking  

---

## 📂 Repository Structure  

# security-audit-internee
