# 🚨 Detection Analysis – File Integrity Monitoring (FIM)

---

## 🔍 Detection Intent

File Integrity Monitoring is designed to detect **unauthorized or unexpected changes** to monitored directories.

In enterprise environments, attackers often:
- Drop malicious files
- Modify configuration files
- Remove traces by deleting artifacts

FIM helps detect these behaviors early.

---

## 📄 File Creation Detection

### Observed Behavior
- New file added to monitored directory
- Agent captured file metadata
- Alert generated and indexed centrally

### SOC Interpretation
This behavior could indicate:
- Malware drop
- Unauthorized script placement
- Insider activity

---

## 🗑️ File Deletion Detection

### Observed Behavior
- File removed from monitored directory
- Deletion event logged by agent
- Alert generated with event context

### SOC Interpretation
Deletion events are critical because they may indicate:
- Evidence tampering
- Cleanup activity after compromise

---

## 🔎 Alert Inspection

The **Inspect** feature allowed deep analysis of:
- File path
- Change type
- Event time
- Agent identity

This level of detail supports investigation and response decisions.

---

## ⚠️ Detection Reliability

- Alerts were consistent
- No false positives observed
- Event lifecycle was accurately tracked

---

## 🧠 Detection Value

FIM provides **high-confidence signals** because file system changes are concrete and measurable, making them valuable for SOC detection pipelines.
