# 🌐 Global Cyber Threat Campaigns & Geopolitical Intelligence (Tableau)

## 📌 Project Overview
The **Global Cyber Threat Campaigns & Geopolitical Intelligence Dashboard** (Template 4 Archetype) delivers macro-level visibility into nation-state cyber campaigns, threat actor origins, targeted countries, cross-border industry impacts, and initial infiltration vectors.

Configured and validated for **Tableau Desktop / Tableau Public (Version 2026.2+)**.

---

## 📂 Project Location & Files
All project files are located at:
`D:\Jaswanth\Tableau\` and `D:\Jaswanth\Tableau\Cybersecurity Threat Intelligence\`

| File Name | Format | Description |
| :--- | :--- | :--- |
| **`Cybersecurity_Threat_Intelligence_Dashboard.twbx`** | Packaged Workbook | **Recommended to open directly!** Contains the Template 4 Geopolitical Dashboard with embedded threat telemetry data. |
| **`Cybersecurity_Threat_Intelligence_Dashboard.twb`** | Tableau Workbook | Pre-configured XML workbook linked to the local dataset. |
| **`cybersecurity_threat_intelligence.csv`** | CSV Dataset | Rich threat intelligence dataset containing **3,500 security incident records** across 2023–2024. |
| **`Data_Dictionary.md`** | Markdown Documentation | Complete data schema, metric formulas, and column definitions. |
| **`README.md`** | Markdown Documentation | This comprehensive project overview and usage guide. |

---

## 📊 Dashboard Visual Architecture (Template 4)

The primary dashboard is titled **`Global Cyber Threat Campaigns Dashboard`** and automatically scales to your display (`Automatic` sizing mode). It features a balanced 2-tier geopolitical layout:

```
+---------------------------------------------------------------------------------------------------+
|               🌐 GLOBAL CYBER THREAT CAMPAIGNS & GEOPOLITICAL INTELLIGENCE                        |
+----------------------------------------------------+----------------------------------------------+
|                                                    |                                              |
|      1. Target Countries Threat Exposure           |     2. Active Nation-State Threat Campaigns  |
|         (Geopolitical Exposure & Avg CVSS)         |        (Ranked Threat Actors by Severity)    |
|                                                    |                                              |
+------------------------------+---------------------+--------+-------------------------------------+
|                              |                              |                                     |
|  3. Cross-Border Sector      |  4. Geopolitical Attack      |  5. Threat Origin                   |
|     Vulnerability ($ Loss)   |     Vectors (Initial Access) |     Nation-States (Attribution)     |
|                              |                              |                                     |
+------------------------------+------------------------------+-------------------------------------+
```

### 1. 🎯 Target Countries Geopolitical Threat Exposure
- **Dimensions**: `Target_Country` (United States, United Kingdom, Germany, Japan, India, Australia, Canada, France, Singapore, Brazil)
- **Measures**: `Count of Incidents` & `Average CVSS Score`
- **Insight**: Highlights which destination nations are facing the highest incident concentration and severity.

### 2. 🥷 Active Nation-State Threat Campaigns
- **Dimensions**: `Threat_Actor` (Volt Typhoon, APT28 Fancy Bear, Cozy Bear, Sandworm, Lazarus Group, LockBit 3.0, BlackCat/ALPHV, Scattered Spider, FIN7)
- **Color Encodings**: `Severity`
  - 🔴 **Critical** (`#e15759`)
  - 🟠 **High** (`#f28e2b`)
  - 🟡 **Medium** (`#edc948`)
  - 🟢 **Low** (`#59a14f`)
- **Insight**: Attributes cyber campaigns to specific threat groups and quantifies their weaponized severity.

### 3. 🏢 Cross-Border Sector Vulnerability & Financial Impact ($)
- **Dimensions**: `Target_Industry` (Energy & Utilities, Financial Services, Healthcare, Government & Public Sector, Defense & Aerospace, Technology, Telecommunications)
- **Measures**: `SUM(Financial_Impact_USD)` formatted in currency (`$`)
- **Insight**: Quantifies monetary risk, critical infrastructure vulnerability, and extortion losses across industries.

### 4. ⚡ Geopolitical Attack Vectors
- **Dimensions**: `Attack_Vector` (Exploitation of Public-Facing App, Phishing & Spearphishing, Zero-Day Exploitation, Compromised Credentials, Supply Chain Compromise, Cloud Misconfiguration)
- **Measures**: `Count of Incidents`
- **Insight**: Details how nation-states and extortion gangs breach security perimeters.

### 5. 🌍 Threat Origin Nation-States Attribution
- **Dimensions**: `Origin_Country` (Russia, China, North Korea, Iran, Eastern Europe, United States, Unknown)
- **Measures**: `Count of Incidents`
- **Insight**: Provides sovereign geopolitical origin attribution for strategic threat modeling.

---

## 🚀 How to Launch
1. Open Windows File Explorer and navigate to **`D:\Jaswanth\Tableau\`**.
2. Double-click on [**`Cybersecurity_Threat_Intelligence_Dashboard.twbx`**](file:///D:/Jaswanth/Tableau/Cybersecurity_Threat_Intelligence_Dashboard.twbx).
3. **Tableau Desktop 2026.2** will open the project directly into the active **Global Cyber Threat Campaigns Dashboard**.
