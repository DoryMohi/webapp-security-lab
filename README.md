# webapp-security-lab
Make the vulnerable web app, secure web app

## Overview
This project demonstrates practical web application security testing using a deliberately vulnerable application. The goal is to identify common web vulnerabilities, analyze their impact, and document appropriate mitigation strategies following industry best practices.

All testing was performed in a **local, legal, and educational environment**.

---

## Technologies & Tools
- OWASP Juice Shop (Docker)
- macOS
- Burp Suite (Community)
- Browser Developer Tools
- Git & GitHub

---

## Security Vulnerabilities Identified

### 1. SQL Injection (Authentication Bypass)
- Bypassed login authentication using crafted SQL payloads
- Gained unauthorized administrative access
- Documented impact and remediation using secure coding practices

Documentation:
- `report/sql-injection.md`
- `report/sql-injection-fix.md`

---

### 2. Cross-Site Scripting (XSS)
- Identified reflected / DOM-based XSS
- Executed JavaScript in the browser via user input
- Demonstrated realistic impact (session exposure)
- Documented mitigation strategies

Documentation:
- `report/xss.md`
- `report/xss_remedy.md`

---

## Tool Usage Note
Manual testing was the primary approach for identifying vulnerabilities in this project.  
HTTP requests and responses were additionally inspected using Burp Suite Community Edition to better understand application behavior during authentication and search requests.

Evidence:
/screenshot/burp_suite_testing.png

## Ethical Disclaimer
All testing was conducted against a deliberately vulnerable application running locally.  
No real systems, users, or data were targeted.  
This project is intended strictly for educational and demonstration purposes.

---

## Skills Demonstrated
- Web application security testing
- OWASP Top 10 vulnerabilities
- Secure coding principles