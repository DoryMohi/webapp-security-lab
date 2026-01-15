## SQL Injection – Authentication Bypass

### Vulnerability Description
The login functionality is vulnerable to SQL Injection due to improper handling of user-supplied input.

### Attack Vector
User input in the login form is directly concatenated into an SQL query without sanitization or parameterization.

### Payload Used
' OR 1=1--
/screenshots/used_credentials.png
### Exploitation Result
The attacker was able to bypass authentication and gain unauthorized access.

### Impact
- Unauthorized access to user accounts
- Potential data leakage or manipulation
- Compromise of application integrity

### OWASP Category
A03:2021 – Injection

### Evidence
![SQL Injection Login Bypass] 
/screenshots/evidence_of_admin_access.png