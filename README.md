# ELK-Stack-SIEM-Lab-Cross-Platform-Log-Analysis
This project has built an Elastic Stack (ELK) infrastructure for centralized log management and security information monitoring (SIEM). The goal is to collect, analyze, and visualize logs from different Operating Systems (Windows and Kali Linux) in real-time.

This lab environment is designed to simulate real SOC (Security Operations Center) operations.

🏗️ Architecture and Topology

SIEM Server: Ubuntu Server (Elasticsearch, Logstash, Kibana)

Log Source 1: Windows 10 (Winlogbeat & Sysmon used)

Log Source 2: Kali Linux (Filebeat & Syslog used)

<img width="2752" height="1536" alt="Gemini_Generated_Image_k2387tk2387tk238" src="https://github.com/user-attachments/assets/92ab72d6-1907-4273-a688-58dc3cf1ec63" />


(You can post the diagram you drew with draw.io here as a picture)

🛠️ Technologies Used

Log Ingestion: Filebeat, Winlogbeat

Log Processing: Logstash (Grok filters)

Storage & Search: Elasticsearch

Visualization: Kibana

Security Monitoring: Sysmon (System Monitor)

📊 Use Cases

The following security events are monitored in this project:

Windows Security:

Failed login attempts (Brute Force Detection - EventID 4625).

New user creation (EventID 4720).

RDP connections.

Linux Security:

SSH login attempts (Failed/Successful Logins).

Sudouse of commands and escalation attempts.

Packet manager (APT) logs.
