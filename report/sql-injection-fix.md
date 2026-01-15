## SQL Injection – Mitigation and Secure Design

### Root Cause
The vulnerability was caused by unsafe string concatenation of user input into SQL queries.

### Mitigation Strategies

#### 1. Parameterized Queries
Prepared statements ensure that user input is treated strictly as data and not executable SQL code.

#### 2. Secure Password Storage
Passwords must be hashed using modern algorithms such as bcrypt or Argon2.

#### 3. Input Validation
User input should be validated for format and length before processing.

#### 4. Principle of Least Privilege
The database account used for authentication should have minimal required permissions.

### Result
These mitigations prevent authentication bypass and protect the application from SQL Injection attacks.

### OWASP Reference
A03:2021 – Injection