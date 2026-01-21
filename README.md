# 🛡️ Basic Log Analysis & Alert Triage using Splunk  

**Author: Piyush Bansal**

This project simulates the work of a **Security Operations Center (SOC)** analyst using **Splunk** to analyze logs, detect suspicious activity, triage alerts, and draft an incident response report.

The goal is to understand how real SOC teams monitor, investigate, and respond to security threats using a SIEM platform.

---

## 🎯 Project Goals

- Set up and explore a SIEM tool (Splunk)
- Analyze incoming security logs (simulated data)
- Detect suspicious activities such as:
  - Failed login attempts
  - Unusual IP behavior
  - Malware-related alerts
- Categorize and prioritize alerts by severity
- Create an incident response report
- Simulate communication with stakeholders
- Learn how SOC teams use dashboards and playbooks

---

## ⚙️ Environment Setup

- **SIEM Tool:** Splunk (Free / Trial version)
- **Data:** Simulated security logs (authentication, system, malware alerts)
- **Role Simulated:** SOC Tier-1 / Tier-2 Analyst

---

## 🔍 What I Did

### 1. Log Exploration
- Ingested sample security logs into Splunk
- Explored data using Search & Reporting
- Identified important fields such as:
  - `user`
  - `src_ip`
  - `host`
  - `action`
  - `timestamp`

---

### 2. Detection & Analysis
Used SPL (Search Processing Language) to detect threats such as:
- Multiple failed login attempts (possible brute-force)
- Same user logging in from multiple IPs
- Malware or suspicious keyword alerts
- High-frequency events from a single source

Example detections:
- Failed logins above a threshold
- Repeated alerts from the same host
- Unusual login patterns

---

### 3. Alert Triage
Each alert was categorized based on:
- Frequency
- Affected user or system
- Potential impact

Severity levels used:
- **Low:** Single or expected failures
- **Medium:** Repeated failed logins
- **High:** Malware detection or account compromise
- **Critical:** Admin account or multiple systems affected

---

### 4. Incident Response Simulation
For identified threats, I documented:
- What happened
- Which systems/users were affected
- Potential impact
- Recommended next steps

Actions included:
- Account lockout
- IP blocking
- System isolation
- Further investigation

---

### 5. Reporting & Communication
- Drafted an incident response report
- Simulated SOC communication to stakeholders
- Explained risks in simple, non-technical language
- Provided actionable recommendations

---

## 📊 What I Learned

- How SOC teams use SIEM tools daily
- How to navigate Splunk efficiently
- How to write meaningful SPL queries
- How to triage alerts instead of panicking
- How to think like a SOC analyst, not just a tool user

---

## 🚀 Future Improvements

- Ingest logs from multiple sources (firewall, IDS, web servers)
- Create custom dashboards
- Automate alerts
- Build SOC playbooks
- Correlate events across log sources


