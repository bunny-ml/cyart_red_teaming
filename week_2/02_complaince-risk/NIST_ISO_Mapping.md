# Framework Cross-Walking: NIST CSF vs. ISO 27001

This document maps organizational security requirements across major frameworks to ensure 100% compliance coverage.

| NIST CSF Function | ISO 27001 Control | Implementation Action |
| :--- | :--- | :--- |
| **Identify (ID.AM)** | A.8.1.1 (Inventory of Assets) | Automated asset discovery via Wazuh agent. |
| **Protect (PR.AC)** | A.9.2.1 (User Registration) | Enforced MFA and Least Privilege via Active Directory. |
| **Detect (DE.CM)** | A.12.4.1 (Event Logging) | Centralized logging via Elastic Stack (ELK). |
| **Respond (RS.RP)** | A.16.1.5 (Response to Incidents) | Automated playbooks for C2 IP blocking. |
| **Recover (RC.RP)** | A.17.1.1 (Continuity Planning) | Daily encrypted off-site backups (AWS S3). |