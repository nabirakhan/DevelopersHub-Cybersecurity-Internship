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


## Security Checklist

- [x] All inputs validated
- [x] Passwords hashed using bcrypt
- [x] JWT used for authentication
- [x] HTTP headers hardened with Helmet
- [x] Logging enabled with Winston
- [x] SQL Injection tested
- [x] XSS vulnerabilities removed
- [x] CSRF protection via csurf
- [x] Secure session cookies (SameSite, HttpOnly)
- [x] CSP configured
- [x] Morgan and Winston used for access and event logging

---

## Tools & Technologies

- OWASP ZAP – Vulnerability scanning  
- Helmet.js – HTTP header security  
- csurf – CSRF protection  
- Winston – Logging system  
- Nmap – Network port scanning  
- connect-mongo – Secure session storage  
- Express.js – Web application framework

---

## Key Learnings

- Performing vulnerability assessments using industry tools
- Implementing middleware-based security in Node.js
- Creating structured audit logs
- Balancing security and usability in web applications
- Applying real-world OWASP Top 10 principles

---

## Conclusion

This internship provided practical experience in ethical hacking, secure web development, and real-world remediation. The final system is significantly more secure and resilient against common web-based attacks while preserving performance and usability.
