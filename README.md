# 🛡️ SOC Home Lab Using Wazuh SIEM 

This project is a self-built **Security Operations Center (SOC)** home lab using the **Wazuh SIEM** platform. It simulates a real-world SIEM environment where logs are collected, analyzed, and responded to using automation techniques such as **VirusTotal integration** and **Active Response**.  

Designed to demonstrate **end-to-end SOC processes** — from agent deployment to file monitoring and threat response — this lab showcases hands-on skills in **incident detection**, **response automation**, and **log analysis**.  

---

## 🧰 Tools & Technologies Used  
- **Wazuh SIEM** (Manager & Agents)  
- **Ubuntu Server 20.04 LTS** (Wazuh Manager)  
- **Windows 10** (Agent)  
- **Ubuntu 22.04** (Agent)  
- **VirusTotal API**  
- **Bash Scripting**  
- **Active Response**  
- **File Integrity Monitoring (FIM)**  

---

## 🧩 Project Structure & Workflow  

### 1️⃣ Wazuh Manager Installation (Ubuntu Server)  
- Installed Wazuh Manager on a dedicated Ubuntu Server.  
- Set up the Wazuh Dashboard, Filebeat, and Elasticsearch stack.  
- Verified the dashboard is accessible and logs are ingested successfully.  

### 2️⃣ Agent Deployment  
- Deployed and registered two agents with the manager:  
  - **Ubuntu Agent** (Linux endpoint)  
  - **Windows Agent** (Windows 10 endpoint)  
- Verified agent connectivity and event forwarding to the Wazuh Manager.  

### 3️⃣ File Integrity Monitoring (FIM)  
**Windows Agent:**  
- Configured to monitor a specific file for unauthorized changes.  
- All file changes (e.g., edits, deletions) are captured and displayed on the Wazuh Dashboard in real time.  

**Ubuntu Agent:**  
- Monitored critical directories (e.g., `/etc`, `/var/log`) for integrity violations.  

### 4️⃣ VirusTotal Integration on Wazuh Server  
- Installed and configured VirusTotal integration on the **Ubuntu Wazuh Manager**.  
- Developed and deployed a script that:  
  - Scans suspicious files or hashes using the VirusTotal API.  
  - Parses the results to identify potential malware.  
- Enabled **Active Response**, allowing the Wazuh Manager to:  
  - Automatically trigger the script when a malicious file or hash is detected.  
  - Take remediation actions like file deletion or alert escalation.  

### 5️⃣ Dashboard Exploration & Log Analysis  
- Explored the Wazuh Dashboard modules:  
  - Security Events  
  - FIM Logs  
  - Agent Status & Performance  
  - Syscheck & Rootcheck  
  - VirusTotal Alerts & Active Response logs  
- Monitored real-time alerts, reviewed triggered rules, and verified response actions.  

---

## 🚨 Key Features Demonstrated  
✅ Complete deployment of Wazuh SIEM environment with multi-agent support  
✅ Real-time File Integrity Monitoring (FIM) on both Windows and Linux endpoints  
✅ Integrated VirusTotal threat intelligence with Wazuh  
✅ Configured Active Response for automated file removal on detection  
✅ Built practical skills in agent deployment, log monitoring, and automated incident response  

---

## 🧠 What I Learned  
- Deep understanding of **SIEM architecture** and real-world SOC workflows  
- Hands-on experience with:  
  - Installing and configuring Wazuh Manager and Agents  
  - deploying Active Response scripts  
  - Setting up VirusTotal
  - Working with log analysis, FIM, and response automation  
- Developed strong **troubleshooting skills** for connectivity, agent registration, and module configurations  

---


