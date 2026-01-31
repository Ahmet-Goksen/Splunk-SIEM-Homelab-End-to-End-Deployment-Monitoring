# Splunk SIEM Homelab: End-to-End Deployment & Monitoring

## Objective
Deploy and configure a fully functional Splunk Enterprise instance from scratch on a Windows host. The goal was to transform raw system telemetry into actionable security and performance insights by building custom dashboards, thereby demonstrating foundational SIEM engineering, log analysis, and threat detection skills.

## Core Setup & Monitoring
This project involved the complete lifecycle of setting up a SIEM on a single host:
1.  **Infrastructure Deployment:** Installed and configured Splunk Enterprise 10.2.0 on a Windows PC, setting up the web interface and core data collection.
2.  **Critical Data Ingestion:** Configured inputs for two vital data streams:
    *   **Windows Event Logs:** Security, System, and Application logs for auditing system activity.
    *   **Windows Performance Counters:** Real-time metrics for `Process`, `Network Interface`, and `TCPv4` objects to monitor system behavior and network health.
3.  **Security-Focused Analysis & Visualization:** Developed custom Splunk Processing Language (SPL) queries to analyze the data and built dedicated dashboards to visualize key security and performance indicators.

## Tools & Data Sources
*   **Primary Platform:** Splunk Enterprise 10.2.0
*   **Operating System:** Windows (Local Host)
*   **Key Data Sources:**
    *   Windows Security Event Logs
    *   Windows Performance Monitor Data (Counters for Process, Network, TCP)
*   **Visualization:** Custom Splunk Dashboards

## Key Achievements & Project Outputs
*   **Operational SIEM Deployment:** Successfully built a working SIEM environment, going from installer to ingesting and searching data.
*   **Strategic Data Selection:** Researched and selected high-value Performance Counters for security monitoring (e.g., `IO Write Bytes/sec` for ransomware detection research, TCP counters for network scans).
*   **Actionable Security Dashboards:** Created visualizations that translate logs and metrics into clear insights:
    *   **Network Traffic Analysis:** Tracked inbound/outbound traffic (`Bytes Sent/Received per sec`) to establish a performance baseline.
    *   **TCP Connection Health:** Monitored `Connections Established`, `Reset`, and `Failed` to identify potential network reconnaissance activity.
    *   **System Event Severity:** Quantified `Warning`, `Error`, and `Critical` logs to triage system health issues.
*   **Practical Threat Research:** Investigated the real-world application of I/O monitoring for detecting ransomware encryption activity, understanding its value and limitations in a modern security context.
![Description of the image](/screenshots/Complete dashboard.png)  
## Skills Demonstrated
*   **SIEM Engineering:** End-to-end installation, configuration, and management of a Splunk instance.
*   **Data Onboarding:** Technical proficiency in configuring inputs for Windows Event Logs and Performance Monitor.
*   **Query Development:** Ability to write and refine SPL queries to filter, analyze, and summarize machine data.
*   **Security Visualization:** Designing dashboards that highlight potential anomalies and security-relevant trends.
*   **Threat Detection Logic:** Applying cybersecurity concepts (like anomaly detection) to build specific monitoring use cases.

---
**See the full technical implementation report:** [detailed_analysis.md](detailed_analysis.md)
