# STRIDE Threat Model: Web Authentication Module

| Threat Category | Potential Attack | Mitigation Strategy | ATT&CK ID |
| :--- | :--- | :--- | :--- |
| **Spoofing** | Session Hijacking via Cookie Theft | Implement Secure/HttpOnly flags | T1539 |
| **Tampering** | SQL Injection in Login Field | Input Validation & Parameterized Queries | T1190 |
| **Repudiation** | User deletes logs after unauthorized access | Centralized WORM Logging (Wazuh) | T1562.002 |
| **Information Disclosure** | Verbose Error Messages leaking DB info | Custom Error Pages / Debug: Off | T1592 |
| **Denial of Service** | Login form Brute Force | Rate Limiting & Account Lockout | T1110 |
| **Elevation of Privilege** | Parameter tampering to access /admin | Role-Based Access Control (RBAC) | T1068 |