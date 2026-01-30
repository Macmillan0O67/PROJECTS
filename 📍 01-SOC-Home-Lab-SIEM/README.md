# SOC Analyst Home Lab – SIEM Monitoring & Incident Response

## 📌 Project Overview
This project simulates a **SOC Level 1 environment** to practice real-world **security monitoring, alert triage, and incident response** using Splunk SIEM.

The lab focuses on detecting suspicious authentication activity, analyzing logs, mapping threats to the **MITRE ATT&CK framework**, and documenting incidents in a SOC-style format.

---

## 🧱 Lab Architecture
- **Windows 10 VM** – Endpoint log source
- **Ubuntu Linux VM** – Server log source
- **Splunk Enterprise** – SIEM platform

Logs from Windows and Linux systems are ingested into Splunk for centralized monitoring and analysis.

---

## 🔍 Use Cases Implemented
- Multiple failed login attempts
- Brute-force attack detection
- Suspicious authentication behavior
- Privilege misuse indicators

---

## 🛠 Tools Used
- Splunk Enterprise (SIEM)
- Windows Event Logs
- Linux Authentication Logs
- MITRE ATT&CK Framework
- VirtualBox / VMware

---

## 🚨 Detection & Alerting
Custom Splunk alerts were created to identify:
- Excessive failed login attempts (Windows & Linux)
- Potential brute-force attacks
- Authentication anomalies

Each alert includes threshold-based triggering and severity classification.

---

## 🧠 Incident Response Workflow
1. Alert validation
2. Log analysis and correlation
3. Threat identification
4. MITRE ATT&CK mapping
5. Severity assessment
6. Incident documentation
7. Remediation recommendations

---

## 📄 Documentation
- SPL queries used for detections
- Alert configuration screenshots
- SOC-style incident reports
- MITRE ATT&CK mappings

---

## 🎯 Skills Demonstrated
- SOC Level 1 Operations
- SIEM Monitoring & Log Analysis
- Alert Triage & Incident Detection
- Threat Analysis
- Security Documentation & Reporting

---
