# DevelopersHub Cybersecurity Internship 🚀

Welcome to my Cybersecurity Internship repository, completed under the mentorship of **DevelopersHub**. This internship focused on identifying, mitigating, and documenting security vulnerabilities in a Node.js-based user management web application.

## 🔐 Internship Overview

**Intern:** Nabira Khan  
**Duration:** 3 Weeks  
**Primary Goal:** Secure a Node.js application by identifying vulnerabilities, implementing protections, and documenting the process.

### 🔗 Target Application
- **GitHub Source:** [Pranavk-official/user-management](https://github.com/Pranavk-official/user-management)
- **Local Server:** `http://localhost:4000`

---

## 🗂️ Week-wise Breakdown

### ✅ Week 1 – Security Assessment
- Performed manual and automated vulnerability scans using OWASP ZAP.
- Key vulnerabilities identified:
  - Broken Access Control on `/admin`
  - No CSRF tokens
  - Missing HTTP security headers
  - Insecure cookie attributes
  - Server info leaks (`X-Powered-By`)
- Tools Used: OWASP ZAP, Chrome Dev Tools, Manual Inspection


---

### ✅ Week 2 – Security Hardening
- Implemented CSP, secure session cookies, and CSRF protection.
- Integrated security middlewares:
  - `helmet`, `csurf`, `connect-mongo`, `nocache`
- Hardened cookies with `HttpOnly`, `SameSite`, `Secure`
- Removed unsafe inline JS and wildcard sources from CSP


---

### ✅ Week 3 – Advanced Security & Finalization
- Simulated Nmap port scanning attacks (`nmap -sV localhost`)
- Integrated **Winston** for structured logging to `security.log`
- Validated final checklist of security controls
- Prepared video demo and all documentation for submission

---

## ✅ Final Report

Includes:
- Summary of all 3 weeks
- Security checklist
- Screenshots of key implementation and scan results
- Logging setup
- Tools used & key learnings

---

## 📋 Security Checklist

```txt
☑ All inputs validated
☑ Passwords hashed using bcrypt
☑ JWT implemented for authentication
☑ Helmet used for secure HTTP headers
☑ Logging enabled with Winston
☑ SQL Injection tested with payloads
☑ XSS vulnerabilities removed
☑ CSRF protection using csurf
☑ Session security set (httpOnly, sameSite)
☑ Morgan and Winston logging active
☑ Content Security Policy applied with Helmet


# 🛠️ Tools & Technologies

- **OWASP ZAP** – Vulnerability scanning  
- **Helmet.js** – HTTP header protection  
- **csurf** – CSRF middleware  
- **Winston** – Logging system  
- **Nmap** – Port scanning  
- **connect-mongo** – Secure session storage  
- **Express.js** – Web application framework  

---

# 🎓 Key Learnings

- Conducting full-stack vulnerability assessments  
- Secure coding practices using modern middleware  
- Building audit logs and detecting suspicious activity  
- Balancing usability with strict security measures  
- Real-world application of OWASP Top 10 principles  

---

# 📷 Screenshots

Screenshots of:
- OWASP ZAP scans  
- Security headers in browser  
- CSRF token verification  
- Log samples in `security.log`  

🗂️ Included in the `screenshots/` directory and embedded in the `Final_Report.md`.

---

# 📽️ Demo

A short video demo of:
- The secured application
- Real-time logging behavior via Winston
- Security headers and CSRF token verification

📁 Available in the root directory or embedded in the `Final_Report.md`.

---

# 🏁 Conclusion

This internship experience provided valuable **hands-on training** in:

- Ethical hacking  
- Secure web development  
- Vulnerability remediation  

It demonstrated how **practical security enhancements** can significantly improve the **resilience of modern web applications** through proper coding standards, middleware usage, and real-world simulation of threats.

---
