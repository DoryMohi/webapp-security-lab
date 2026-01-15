### CROSS-SITE SCRIPTING (XSS)

### Type
Reflected / DOM-Based XSS

### Vulnerability Description
User-controlled input is reflected into the web page without proper output encoding. As a result, the browser interprets the input as executable code, allowing arbitrary JavaScript execution in the victim’s browser.

### Payload Used
<img src=x onerror=alert(1)>

### Exploitation Result
The injected JavaScript payload was executed successfully in the browser, confirming the presence of a Cross-Site Scripting vulnerability.

### Impact
	•	Execution of arbitrary JavaScript in the client’s browser
	•	Access to sensitive data such as session cookies or authentication tokens
	•	Session hijacking and user impersonation
	•	Potential account takeover and other client-side attacks

### Realistic Attack Demonstration
During testing, it was verified that injected JavaScript could access <document.cookie>, demonstrating that an attacker could potentially hijack authenticated user sessions. For ethical reasons, sensitive values were not exfiltrated, stored, or shared.

### OWASP Category
A03:2021 – Injection

### Evidence
Screenshot showing JavaScript alert execution captured during testing.
/screenshots/xss_proof.png 