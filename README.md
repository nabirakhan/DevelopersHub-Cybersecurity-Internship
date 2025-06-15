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

📄 [Week 1 Report](./reports/Week-1-Security-Assessment.md)

---

### ✅ Week 2 – Security Hardening
- Implemented CSP, secure session cookies, and CSRF protection.
- Integrated security middlewares:
  - `helmet`, `csurf`, `connect-mongo`, `nocache`
- Hardened cookies with `HttpOnly`, `SameSite`, `Secure`
- Removed unsafe inline JS and wildcard sources from CSP

📄 [Week 2 Report](./reports/Week-2-Security-Hardening.md)

---

### ✅ Week 3 – Advanced Security & Finalization
- Simulated Nmap port scanning attacks (`nmap -sV localhost`)
- Integrated **Winston** for structured logging to `security.log`
- Validated final checklist of security controls
- Prepared video demo and all documentation for submission

📄 [Week 3 Report](./reports/Week-3-Advanced-Security.md)

---

## ✅ Final Report

Includes:
- Summary of all 3 weeks
- Security checklist
- Screenshots of key implementation and scan results
- Logging setup
- Tools used & key learnings

📄 [Final_Report.md](./Final_Report.md)

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
