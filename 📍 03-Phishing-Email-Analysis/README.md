# 📧 Phishing Email Investigation – SOC Level 1 Simulation

![SOC](https://img.shields.io/badge/Role-SOC%20Level%201-blue)
![Project Type](https://img.shields.io/badge/Project-Cybersecurity-red)
![MITRE ATT&CK](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📌 Project Overview

This project simulates a real-world **SOC Level 1 phishing email investigation**.  
The objective was to analyze a suspicious email, extract Indicators of Compromise (IOCs), classify the attack type, and map findings to the MITRE ATT&CK framework.

This project demonstrates practical SOC triage methodology used in Security Operations Centers (SOC).

---

## 🎯 Objectives

- Perform email header analysis
- Identify spoofed domains and sender anomalies
- Extract and investigate malicious URLs
- Classify phishing attack type
- Map findings to MITRE ATT&CK techniques
- Document findings in SOC report format

---

## 🔍 Investigation Process

### 1️⃣ Email Header Analysis
- Analyzed SPF and DKIM authentication results
- Identified authentication failures
- Reviewed "Received" headers for source tracing

### 2️⃣ Sender & Domain Investigation
- Traced originating IP address
- Checked domain registration details
- Verified domain reputation
- Identified spoofed/lookalike domains

### 3️⃣ URL Analysis
- Extracted embedded URLs
- Performed reputation analysis
- Checked redirection behavior
- Identified credential harvesting intent

### 4️⃣ Threat Classification
- Categorized phishing subtype
- Documented Indicators of Compromise (IOCs)
- Assigned severity level

---

## 🧠 MITRE ATT&CK Mapping

| Technique | Technique ID |
|-----------|-------------|
| Phishing | T1566 |
| Credential Harvesting | T1056 |

Framework Reference: MITRE ATT&CK Enterprise Matrix

---

## 🛠 Tools & Technologies Used

- Email Header Analyzer
- WHOIS Lookup
- URL Reputation Platforms
- Threat Intelligence Sources
- MITRE ATT&CK Framework
- SOC L1 Triage Methodology

---

## 📊 Indicators of Compromise (IOCs)

- Malicious Sender IP: `185.220.101.45`
- Spoofed Domain: `micr0soft-support.com`
- Malicious URL: `[http://malicious-link.com/logi](http://secure-microsoft-login.com/verify-account)`
- Authentication Failure: SPF & DKIM Failed



---


```

---

