 🛡️ Incident Report – Service Persistence Detection

 📌 Incident Summary
A suspicious Windows service configuration change was detected by Wazuh SIEM during SOC home lab monitoring. The alert indicates potential persistence behavior commonly used by attackers to maintain system access.


 🖥️ Detection Source
- Platform: Wazuh SIEM
- Module: Security Events Monitoring
- Agent: HACKTHEWORLD (Windows Server 2016)
- Detection Time: Feb 27, 2026


🚨 Alert Details
- Rule ID: 61104
- Alert Level: 3
- Event Description: Service startup type was changed
- MITRE ATT&CK Technique: Persistence (T1543 – Create or Modify System Process)


🔎 Investigation Steps
1. Reviewed alert from Wazuh Security Events dashboard.
2. Identified affected host and agent ID.
3. Checked related Windows event logs.
4. Confirmed service configuration modification activity.
5. Validated activity as part of controlled attack simulation.


🧠 Analysis
Changing service startup configuration is a known persistence technique used by attackers to execute malicious processes automatically after system reboot.


 ✅ Conclusion
The alert successfully demonstrated Wazuh SIEM's capability to detect persistence-related system modifications. The activity was intentionally simulated within a SOC home lab environment for learning and detection analysis purposes.

---

## 📷 Evidence
Refer to screenshots folder for related alert evidence:
`screenshots/service-persistence-alert.png`
