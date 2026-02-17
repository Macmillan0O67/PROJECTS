# 📧 Phishing Incident Investigation Report  

**Incident Title:** Financial Institution Impersonation – Credential Harvesting Attempt  
**Incident Type:** Phishing Attack  
**Environment:** Corporate Email Environment (Simulated Lab)  
**Detection Method:** User Reported + SOC Triage  
**Incident Date:** 12 February 2026  
**Analyst:** Jibin Jose  
**Report Version:** 1.0  

---

# 1. Executive Summary

A phishing email impersonating a financial institution was identified within the corporate email environment. The attack attempted to harvest user credentials through a malicious URL redirect chain.

The incident was reported by the end user and escalated to the Security Operations Center (SOC) for investigation and response. Indicators of Compromise (IOCs) confirmed malicious infrastructure involvement.

The threat was successfully contained through domain blocking and email security rule updates.

---

# 2. Incident Overview

## 2.1 Attack Type
- Credential Harvesting Phishing Campaign

## 2.2 Attack Vector
- Email-based social engineering
- Malicious embedded hyperlink
- Domain impersonation

## 2.3 Impact Assessment
- No confirmed credential compromise
- Attempted unauthorized access
- Moderate reputational and operational risk

---

# 3. Indicators of Compromise (IOCs)

- Suspicious sender domain (Lookalike financial institution domain)
- Malicious URL redirect chain
- Sender IP flagged by threat intelligence sources
- SPF / DKIM authentication failure
- Domain recently registered

---

# 4. Timeline of Events

| Time     | Action Taken        |
|----------|--------------------|
| 11:05 AM | Phishing email received |
| 11:08 AM | User reported suspicious email |
| 11:12 AM | SOC initiated triage investigation |
| 11:18 AM | URL analysis confirmed credential harvesting page |
| 11:25 AM | Malicious domain blocked at gateway |

---

# 5. Investigation Details

## 5.1 Email Header Analysis
- SPF: Failed
- DKIM: Failed
- DMARC: Quarantine policy triggered
- Sender domain impersonated legitimate financial institution

## 5.2 URL Analysis
- Embedded hyperlink redirected through multiple domains
- Final landing page hosted credential harvesting form
- Domain reputation flagged as malicious by OSINT sources

## 5.3 Infrastructure Analysis
- Hosting IP associated with prior phishing campaigns
- Newly registered domain (< 7 days old)

---

# 6. Containment Actions

- Blocked malicious domain at email gateway
- Added URL to proxy blacklist
- Updated email filtering rules
- Notified affected user
- Conducted awareness communication to employees

---

# 7. MITRE ATT&CK Mapping

| Technique | Technique ID |
|-----------|--------------|
| Phishing | T1566 |
| Credential Harvesting | T1056 |
| Domain Impersonation | T1583 |

---

# 8. Risk Assessment

| Category | Risk Level |
|----------|------------|
| Confidentiality | Medium |
| Integrity | Low |
| Availability | Low |
| Overall Severity | Medium |

---

# 9. Recommendations

- Enable strict DMARC enforcement policy (Reject)
- Implement advanced email sandboxing
- Deploy URL rewriting and time-of-click protection
- Conduct periodic phishing simulation training
- Strengthen user awareness programs
- Monitor newly registered domains targeting organization brand

---

# 10. Lessons Learned

- User awareness played a critical role in early detection
- Email authentication enforcement requires improvement
- Threat intelligence integration enhances response speed

---

# 11. Conclusion

The phishing attempt was successfully detected and contained without confirmed compromise. Early user reporting and SOC response minimized potential damage.

Improving email authentication controls and enhancing phishing defense mechanisms will further reduce organizational risk exposure.

---

# 12. Disclaimer

This investigation was conducted in a simulated lab environment for cybersecurity training and portfolio demonstration purposes.
