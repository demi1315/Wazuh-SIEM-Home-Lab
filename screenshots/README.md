# 📸 Screenshot Reference – Wazuh FIM Lab

All screenshots were captured during a controlled home lab environment and are provided strictly for documentation purposes.

---

## 🧱 Agent Configuration

- **ossec-conf-edit.png**  
  Editing `ossec.conf` with Administrator privileges to add a new FIM path.

- **fim-path-added.png**  
  FIM configuration updated to include `WAZUH_TEST` directory.

---

## 🔄 Agent Restart

- **agent-restart.png**  
  Restarting Wazuh Agent to apply configuration changes.

---

## 📄 File Creation Detection

- **file-created.png**  
  Creation of `test-1.txt` inside monitored directory.

- **fim-create-alert.png**  
  Alert generated for new file creation.

- **alert-inspect-create.png**  
  Inspection of file creation alert details.

---

## 🗑️ File Deletion Detection

- **file-deleted.png**  
  Deletion of test file from monitored directory.

- **fim-delete-alert.png**  
  Alert generated for file deletion event.

---

## 📝 Notes

- No real system files were altered  
- All changes were intentional  
- Events validate FIM detection lifecycle  
