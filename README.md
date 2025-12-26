# 🛡️ Wazuh SIEM Home Lab – Endpoint Monitoring & File Integrity Monitoring (FIM)

This repository documents a **SOC-style Wazuh SIEM home lab** focused on **endpoint monitoring and File Integrity Monitoring (FIM)**.  
The project demonstrates how file system changes on a Windows endpoint are detected, logged, and analyzed centrally using Wazuh.

The lab simulates how **SOC analysts monitor unauthorized or unexpected file changes**, which is a critical detection use case in enterprise environments.

---

## 🎯 Project Objective

The objective of this project was to:

- Deploy Wazuh SIEM in a home lab environment  
- Onboard a Windows endpoint using Wazuh Agent  
- Configure **File Integrity Monitoring (FIM)** manually  
- Detect file creation, modification, and deletion events  
- Analyze alerts and metadata in the Wazuh Manager  
- Understand how endpoint telemetry supports incident detection  

---

## 🧱 Lab Architecture

Windows Endpoint (Wazuh Agent) → Wazuh Manager → Wazuh Dashboard


| Component | Description |
|--------|-------------|
| SIEM Platform | Wazuh |
| Manager OS | Linux |
| Endpoint | Windows |
| Agent | Wazuh Agent |
| Use Case | Endpoint Monitoring & FIM |

---

## 🧭 SOC Workflow Demonstrated

1️⃣ Endpoint telemetry collection  
2️⃣ Manual FIM configuration  
3️⃣ File system activity generation  
4️⃣ Centralized alert ingestion  
5️⃣ Alert inspection & validation  
6️⃣ Event lifecycle analysis  

---

## 🔎 Key Security Use Case

**File Integrity Monitoring (FIM)** is used to detect:

- Unauthorized file creation  
- Unexpected file modification  
- Malicious or accidental file deletion  

This is especially important for:
- Configuration files  
- Application directories  
- Sensitive system folders  

---

## ⚠️ Ethical Disclaimer

This lab was conducted **strictly in a controlled home lab environment** for educational purposes.

- No production systems were monitored  
- No real user data was involved  
- All file changes were intentional and authorized  

---

📌 *This repository is part of my cybersecurity portfolio and demonstrates hands-on experience with SIEM-based endpoint monitoring and file integrity detection.*




