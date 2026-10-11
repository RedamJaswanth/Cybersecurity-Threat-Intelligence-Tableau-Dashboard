# 🛡️ SOC Operations & Live Incident Response Center (Tableau)

## 📌 Project Overview
The **SOC Operations & Live Incident Response Center** provides real-time security operations visibility into active threat alerts, containment funnel lifecycles, attack vector surge velocity, and live telemetry.

Validated for **Tableau Desktop / Tableau Public (Version 2026.2+)**.

---

## 📂 Project Location & Files
All project files are located at:
`D:\Jaswanth\Tableau\` and `D:\Jaswanth\Tableau\Cybersecurity Threat Intelligence\`

| File Name | Format | Description |
| :--- | :--- | :--- |
| **`Cybersecurity_Threat_Intelligence_Dashboard.twbx`** | Packaged Workbook | **Recommended to open directly!** Contains the full SOC Operations Dashboard with embedded telemetry data. |
| **`Cybersecurity_Threat_Intelligence_Dashboard.twb`** | Tableau Workbook | Pre-configured XML workbook linked to local dataset. |
| **`cybersecurity_threat_intelligence.csv`** | CSV Dataset | Rich threat intelligence dataset containing **3,500 security incident records**. |
| **`index.html`** | Interactive Web App | 60 FPS live animated SOC command center application with wave velocity lines, triage funnel, and live rolling IOC telemetry. |
| **`dashboard_reference.jpg`** | Reference Image | High-resolution visual mockup. |
| **`Data_Dictionary.md`** | Markdown Documentation | Complete data schema, metric formulas, and column definitions. |
| **`README.md`** | Markdown Documentation | Project overview and usage guide. |

---

## 📊 Dashboard Visual Architecture

The dashboard is titled **`SOC OPERATIONS & LIVE INCIDENT RESPONSE`** and features:

```
+---------------------------------------------------------------------------------------------------+
|               🚨 SOC OPERATIONS & LIVE INCIDENT RESPONSE CENTER                                   |
+-------------------+-------------------+-------------------+---------------------------------------+
|  ACTIVE ALARMS    |  BLOCKED ATTACKS  |  CONTAINED INC.   |  UNDER REMEDIATION                    |
|  482 [CRITICAL]   |  34,912           |  129              |  67                                   |
+-------------------+-------------------+-------------------+---------------------------------------+
|                                       |                                                           |
|  1. Attack Surge Velocity Timeline    |  2. Incident Response Funnel Stage Pipeline               |
|     (Multi-Vector Wave Tracking)      |     (Detection -> Triage -> Containment -> Remediation)   |
|                                       |                                                           |
+---------------------------------------+-------------------+---------------------------------------+
|                                       |                   |                                       |
|  3. Live IOC Telemetry Feed           |  4. Response MTTR |  5. Industry SLA                      |
|     (Artifacts, Hashes, IP Feeds)     |     by Severity   |     Distribution                      |
|                                       |                   |                                       |
+---------------------------------------+-------------------+---------------------------------------+
```

### 1. 🚨 Top SOC Metric Badges
- **Active Alarms:** 482 Critical
- **Blocked Attacks:** 34,912
- **Contained Incidents:** 129
- **Under Remediation:** 67

### 2. 📈 Attack Surge Velocity Timeline
- Wave velocity across threat vectors (*Phishing, Zero-Day, Exploitation of Public Apps, Ransomware*).

### 3. 🔻 Incident Response Funnel Pipeline
- 7-stage operational lifecycle: *Detection (511) ➔ Triage (403) ➔ Investigation (288) ➔ Containment (129) ➔ Remediation (67) ➔ Recovery (54) ➔ Closed (198)*.

### 4. 📡 Live Indicators of Compromise (IOC Feed)
- Real-time table of malicious IPs, file hashes (SHA256), and C2 beacon endpoints with severity classification (*[CRITICAL], [HIGH], [MEDIUM]*).

### 5. ⏱️ Response Latency (MTTR) by Severity
- Mean Time to Respond benchmarks by severity tier.

---

## 🚀 How to Launch
1. **In Tableau Desktop:** Double-click on [**`Cybersecurity_Threat_Intelligence_Dashboard.twbx`**](file:///D:/Jaswanth/Tableau/Cybersecurity_Threat_Intelligence_Dashboard.twbx).
2. **In Browser:** Double-click on [**`index.html`**](file:///D:/Jaswanth/Tableau/index.html) for the live animated 60 FPS version!
