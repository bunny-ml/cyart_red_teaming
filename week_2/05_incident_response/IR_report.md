# Incident Report: VSFTPD Backdoor Exploitation (T1190)

**Date:** 2026-02-6  
**Severity:** Critical  
**Status:** Resolved  

## 1. Executive Summary
An unauthorized remote access attempt was detected targeting the VSFTPD service on the staging server. The attacker successfully gained a root shell.

## 2. Timeline
- **11:00:** Attack initiated (Metasploit exploit/unix/ftp/vsftpd_234_backdoor).
- **11:01:** Wazuh generated "Level 12" Alert: Potential Backdoor Detected.
- **11:05:** Containment started. Attacker IP `192.168.31.105` blocked via CrowdSec.


## 3. Evidence Collection
- **Log Source:** `/var/log/vsftpd.log`
- **Artifacts:** Network netstat showing connection on port 6200.

## 4. Remediation & Lessons Learned
- **Action:** Disabled VSFTPD 2.3.4 and migrated to a hardened SFTP configuration.
- **Lesson:** Vulnerability scanning (OpenVAS) should have flagged this prior to deployment.