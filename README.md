# 🛡️ Wazuh SIEM Lab – Multi-Source Security Monitoring with Wazuh

## 📌 Project Overview

This project demonstrates the deployment of a Security Information and Event Management (SIEM) lab using **Wazuh** to monitor multiple log sources, detect suspicious activities, and visualize security events through custom dashboards.

The lab collects and analyzes logs from:

- Windows Endpoint
- Ubuntu Linux Endpoint
- Simulated Firewall (pfSense-style logs)

Custom correlation rules were created to detect brute-force attacks and suspicious command execution, providing a practical SOC analyst workflow.

---

## 🎯 Objectives

- Deploy a functional Wazuh SIEM
- Onboard multiple log sources
- Parse and normalize security logs
- Build useful SOC dashboards
- Create custom detection rules
- Investigate alerts generated from simulated attacks

---

## 🛠️ Technologies Used

- Wazuh
- Ubuntu Server
- Windows 10
- VirtualBox
- Sysmon
- Windows Event Logs
- Linux Audit Logs
- OpenSearch Dashboards

---

## 🏗️ Lab Architecture

![Architecture](diagrams/architecture-diagram.png)

---

## 📊 Screenshots

### Wazuh Dashboard Overview

![Dashboard](screenshots/dashboard-overview.png)

---

### Connected Agents

![Agents](screenshots/agent-page.png)

---

### Windows Event Data

![Windows Events](screenshots/windows-event-data.png)

---

### Authentication Dashboard

Shows successful vs failed logins.

![Authentication](screenshots/authentication-dashboard.png)

---

### Network Traffic Dashboard

![Traffic](screenshots/network-traffic-dashboard.png)

---

### Most Frequent Processes

![Processes](screenshots/most-frequent-process.png)

---

## 🚨 Detection Rules

### Rule 100200 — Multiple Failed Logins

Detects 5 or more failed authentication attempts within 5 minutes.

![Rule100200](screenshots/correlation-rule-100200.png)

---

### Rule 100300 — Living-off-the-Land Detection

Detects suspicious execution of built-in Windows tools commonly abused by attackers.

![Rule100300](screenshots/correlation-rule-10300.png)

---

## 📈 Key Achievements

- Successfully deployed a working Wazuh SIEM lab
- Integrated multiple log sources
- Built custom SOC dashboards
- Created correlation rules for attack detection
- Investigated alerts from generated events
- Documented the complete implementation process

---

## 📄 Documentation

Project Report:

`docs/SIEM-Lab-Project-Report.pdf`

Presentation Slides:

`docs/SIEM-Lab-Presentation.pptx`

---

## 👨🏽‍💻 Author

**Boluwatife Makinde**

Aspiring SOC Analyst | Cybersecurity Learner

LinkedIn:
www.linkedin.com/in/boluwatife-makinde-571ba3378

GitHub:
https://github.com/CyberTife
