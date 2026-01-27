# 🔍 SOC Log Analysis & Threat Detection using Splunk

This project demonstrates practical experience in Security Information and Event Management (SIEM) by analyzing Windows Security Event Logs using **Splunk Enterprise**.

## 🚀 Project Overview
The objective was to ingest raw security logs and use **Search Processing Language (SPL)** to identify potential security threats, such as brute-force attacks and unauthorized access attempts.

## 🛠️ Tools & Skills Demonstrated
- **SIEM Platform:** Splunk Enterprise
- **Data Source:** `WinEventLog:Security` (Windows Security Logs)
- **Technical Skills:** Log Analysis, SPL Querying, Data Visualization, Incident Monitoring.

## 📊 Analysis Breakdown

### 1. Statistical Log Analysis
I used SPL to aggregate event counts by their unique EventCodes to understand the overall security posture of the system.
- **Query:** `index=main sourcetype="WinEventLog:Security" | stats count by EventCode`
![Event Analysis](S-1.png)

### 2. Identifying Failed Login Attempts (Brute Force Monitoring)
Monitoring **EventCode 4625** is critical for detecting potential unauthorized access. I filtered logs to isolate these events for deeper investigation.
- **Query:** `index=main EventCode=4625`
![Failed Logins](S-2.png)

### 3. Data Visualization
Transformed raw log data into an **Area Chart** to visualize event frequency and identify abnormal spikes in system activity.
![Visualization](S-3.png)

---
**Summary:** This project highlights my ability to use industry-standard SIEM tools to perform proactive security monitoring and data-driven threat analysis.
