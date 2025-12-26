# 🔎 SOC Assessment Notes – Wazuh Endpoint Monitoring & FIM

---

## 🎯 Assessment Objective

This assessment was conducted to **simulate a SOC analyst workflow** focused on detecting file system changes on an endpoint using **Wazuh File Integrity Monitoring (FIM)**.

The goal was to understand how:
- Endpoint-side configuration enables monitoring
- File system events generate alerts
- SOC analysts validate and interpret these alerts centrally

---

## 🧱 Environment Overview

- Wazuh Manager deployed on Linux  
- Wazuh Agent installed on Windows endpoint  
- Agent successfully registered and connected  
- Alerts visualized through Wazuh Dashboard  

---

## 🧭 Assessment Methodology

The assessment followed a **realistic SOC testing sequence**.

---

### 📥 Step 1 — Agent Configuration Review

The Wazuh agent configuration file (`ossec.conf`) was accessed on the Windows endpoint.

- File was opened using **Notepad with Administrator privileges**
- FIM configuration section was identified
- A new directory was added for monitoring

This step simulates how SOC teams define **critical paths for integrity monitoring**.

---

### 🗂️ Step 2 — FIM Path Configuration

A new directory named **WAZUH_TEST** was added to the FIM configuration inside `ossec.conf`.

This explicitly instructed the agent to monitor this folder for:

- File creation
- File modification
- File deletion

---

### 🔄 Step 3 — Agent Restart

After updating the configuration:

- The Wazuh Agent service was restarted
- Configuration changes were applied
- Agent resumed secure communication with the manager

Restarting the agent ensured the new FIM rules became active.

---

### 📄 Step 4 — File Creation Event

A test file named **test-1** was created inside the `WAZUH_TEST` directory.

This action simulated:
- Unauthorized file introduction
- Potential malicious payload placement

---

### 🚨 Step 5 — Alert Detection & Inspection

The Wazuh Manager detected the file creation event and generated an alert.

Using the **Inspect** option in the dashboard, the alert details were reviewed, including:
- File path
- Event type (creation)
- Timestamp
- Agent information

---

### 🗑️ Step 6 — File Deletion Event

The `test-1.txt` file was deleted from the monitored directory.

After refreshing the dashboard:
- A **file deletion alert** was generated
- The event lifecycle was successfully validated

---

## ✅ Key Observations

- FIM rules were applied correctly  
- Agent detected file creation and deletion  
- Alerts were transmitted in near real-time  
- Detailed metadata was available for analysis  
- SOC visibility into endpoint activity was confirmed  

---

## 📘 Purpose of This Document

This document demonstrates **practical endpoint monitoring and SOC validation skills**, not theoretical configuration steps.




