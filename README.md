# DevelopersHub Cybersecurity Internship

Welcome to my Cybersecurity Internship repository, completed under the mentorship of **DevelopersHub**. This internship focused on identifying, mitigating, and documenting security vulnerabilities in a Node.js-based user management web application.

## Internship Overview

**Intern:** Nabira Khan  
**Duration:** 6 Weeks  
**Primary Goal:** Secure a Node.js application by identifying vulnerabilities, implementing protections, and documenting the process.

### Target Application
- **GitHub Source:** [Pranavk-official/user-management](https://github.com/Pranavk-official/user-management)
- **Local Server:** `http://localhost:4000`

---

## Week-wise Breakdown

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

### ✅ Week 4 – Advanced Threat Detection & Web Security Enhancements
- Enabled rate limiting using `express-rate-limit` to prevent brute-force attacks
- Configured CORS to allow only trusted domains
- Implemented API key-based authentication for protected endpoints
- Applied security headers:
  - Content-Security-Policy (CSP)
  - Strict-Transport-Security (HSTS)
  - X-Content-Type-Options, X-Frame-Options, Referrer-Policy
- Deployed Fail2Ban for real-time intrusion detection and blocking

---

### ✅ Week 5 – Ethical Hacking & Exploiting Vulnerabilities
- Used Kali Linux for ethical hacking simulation
- Performed reconnaissance and enumeration
- Detected SQL Injection vulnerability using SQLMap and fixed using prepared statements
- Implemented CSRF protection using `csurf` and validated using Burp Suite
- Documented vulnerabilities found and corresponding mitigations

---

### ✅ Week 6 – Security Audits & Final Deployment
- Performed security scans using OWASP ZAP, Nikto, and Lynis
- Checked OWASP Top 10 compliance and resolved flagged issues
- Added dependency scanning with `npm audit` and GitHub Dependabot
- Scanned and hardened Docker container using `docker scan` and `trivy`
- Performed final penetration test using Burp Suite
- Final application secured and deployed in Docker environment
- Recorded and submitted final video presentation demonstrating all security features

---

## Security Checklist

- [x] All inputs validated
- [x] Passwords hashed using bcrypt
- [x] JWT used for authentication
- [x] HTTP headers hardened with Helmet
- [x] Logging enabled with Winston
- [x] SQL Injection tested and fixed
- [x] XSS vulnerabilities removed
- [x] CSRF protection via csurf
- [x] Secure session cookies (SameSite, HttpOnly, Secure)
- [x] CSP configured
- [x] Morgan and Winston used for access and event logging
- [x] API authentication via API key
- [x] Rate limiting to prevent brute-force attacks
- [x] Fail2Ban installed for intrusion detection
- [x] CORS configured to allow only trusted domains
- [x] Final penetration testing conducted and passed
- [x] Docker container scanned and secured

---

## Tools & Technologies

- OWASP ZAP – Vulnerability scanning  
- Helmet.js – HTTP header security  
- csurf – CSRF protection  
- Winston – Logging system  
- Nmap – Network port scanning  
- connect-mongo – Secure session storage  
- Express.js – Web application framework  
- SQLMap – SQL Injection testing  
- Burp Suite – Vulnerability analysis  
- Fail2Ban – Brute-force protection  
- express-rate-limit – API rate limiting  
- Docker & Trivy – Container security  

---

## Key Learnings

- Performing vulnerability assessments using industry tools
- Implementing middleware-based security in Node.js
- Creating structured audit logs and alerts
- Defending against OWASP Top 10 vulnerabilities
- Securing APIs through headers, tokens, and rate limits
- Conducting penetration testing in a real-world environment
- Hardening Docker deployments and scanning for vulnerabilities

---

## Conclusion

This internship provided hands-on experience in web security, vulnerability detection, ethical hacking, and secure deployment practices. The final version of the application is significantly more resilient to modern attack techniques, compliant with OWASP standards, and suitable for production environments.

