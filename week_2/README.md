# Advanced Security Operations & Threat Research Lab
A comprehensive end-to-end cybersecurity project demonstrating expertise in Threat Modeling, Defensive Engineering, and Incident Response.

## 🛠️ Tech Stack & Tools
* **SIEM/XDR:** Wazuh, Elastic Security, Security Onion
* **Threat Intel:** MITRE ATT&CK, MISP, Sigma Rules
* **Forensics/IR:** Velociraptor, REMnux, SANS IR Framework
* **Infrastructure:** Metasploitable2, Windows Server (Lab), Suricata IDS

## 🚀 Key Project Milestones

### 1. Threat Modeling & Attack Surface Mapping
* **STRIDE Analysis:** Performed a deep-dive threat model on a multi-tier web application.
* **ATT&CK Mapping:** Aligned detected adversary behaviors (T1566, T1059) to defensive controls.

### 2. Detection Engineering (Sigma & IDS)
* **Rule Development:** Authored custom Sigma rules to detect suspicious PowerShell execution.
* **Network Defense:** Implemented Suricata rules to identify and drop C2 traffic patterns.

### 3. Incident Response & Malware Analysis
* **Full-Cycle IR:** Conducted a capstone "Live Fire" exercise: 
    * *Detection* (Wazuh) -> *Containment* (CrowdSec) -> *Remediation* (SANS Template).
* **Static Analysis:** Binary analysis of malicious samples using `strings` and `peframe`.

## 📊 Risk Management
* **Quantitative Analysis:** Calculated ALE for Ransomware scenarios.
* **Frameworks:** Implemented NIST CSF (Identify/Protect) and ISO 27001 control mappings.
