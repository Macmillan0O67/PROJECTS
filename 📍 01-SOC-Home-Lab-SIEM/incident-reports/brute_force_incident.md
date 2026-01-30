# Security Incident Report – Brute Force Attack

## Incident ID
SOC-INC-001

## Incident Type
Brute Force Authentication Attempt

## Detection Source
Splunk SIEM

## Severity
Medium

---

## 🧾 Executive Summary
Splunk SIEM generated an alert indicating multiple failed authentication attempts against a Windows endpoint within a short time frame. Analysis confirmed a brute-force attempt targeting a local user account. No successful login was observed.

---

## ⏱ Timeline of Events
| Time (UTC) | Event |
|----------|------|
| 10:15 | Multiple failed login attempts detected |
| 10:17 | Splunk alert triggered |
| 10:20 | SOC analyst began investigation |
| 10:30 | Incident classified and documented |

---

## 🔍 Indicators of Compromise (IOCs)
- Repeated failed login events (Event ID 4625)
- Targeted local user account
- Abnormal authentication frequency

---

## 🧠 MITRE ATT&CK Mapping
- **T1110 – Brute Force**

---

## 📊 Impact Assessment
- No account compromise detected
- Potential risk of credential exposure if attack continued
- Increased authentication load on endpoint

---

## 🛡 Remediation & Recommendations
- Enforce account lockout policies
- Strengthen password complexity requirements
- Enable multi-factor authentication (MFA)
- Monitor authentication logs continuously
- Implement IP-based rate limiting where applicable

---

## 📌 Incident Status
Closed – No further malicious activity observed

---
