# 📖 Data Dictionary: Cybersecurity Threat Intelligence

This dataset contains telemetry, incident response metrics, and MITRE ATT&CK mapping for 3,500 enterprise security events.

| Column Name | Data Type | Tableau Role | Description & Examples |
| :--- | :--- | :--- | :--- |
| `Incident_ID` | String | Dimension | Unique identifier for the incident (e.g., `CTI-2024-00124`). |
| `Timestamp` | Datetime | Dimension | Exact timestamp when the event was logged. |
| `Date` | Date | Dimension | Date representation for temporal rollups (Year, Quarter, Month, Day). |
| `Threat_Actor` | String | Dimension | Attributed threat actor group (e.g., `APT28 (Fancy Bear)`, `LockBit 3.0`, `Volt Typhoon`, `Lazarus Group`). |
| `Threat_Actor_Type` | String | Dimension | Categorization of the adversary: `Nation-State (APT)`, `Ransomware-as-a-Service`, `Cybercrime Syndicate`, `Hacktivist`. |
| `Origin_Country` | String | Dimension (Geo) | Suspected origin country of the adversary (e.g., `Russia`, `China`, `North Korea`, `Iran`). |
| `Target_Country` | String | Dimension (Geo) | Destination country targeted in the campaign (e.g., `United States`, `Germany`, `United Kingdom`, `Japan`, `India`). |
| `Target_Industry` | String | Dimension | Industry vertical targeted (e.g., `Financial Services`, `Healthcare`, `Energy & Critical Infrastructure`, `Defense`). |
| `Attack_Vector` | String | Dimension | Mechanism used to gain entry (e.g., `Phishing & Spearphishing`, `Exploit Public-Facing App`, `Zero-Day Vulnerability`). |
| `MITRE_Tactic` | String | Dimension | High-level tactical phase in MITRE ATT&CK enterprise matrix (e.g., `Initial Access`, `Persistence`, `Credential Access`, `Impact`). |
| `MITRE_Technique_ID` | String | Dimension | Canonical MITRE ATT&CK technique code (e.g., `T1566`, `T1190`, `T1078`, `T1486`). |
| `MITRE_Technique_Name` | String | Dimension | Technique description (e.g., `Phishing: Spearphishing Attachment`, `Data Encrypted for Impact`). |
| `Malware_Family` | String | Dimension | Primary malware or tool detected (e.g., `Cobalt Strike Beacon`, `Mimikatz`, `LockBit 3.0 Encryptor`, `WhisperGate Wiper`). |
| `Severity` | String | Dimension | Risk severity rating: `Critical`, `High`, `Medium`, `Low`. |
| `CVSS_Score` | Real (Float) | Measure | Common Vulnerability Scoring System base score (1.0 to 10.0). |
| `IOC_Type` | String | Dimension | Indicator of Compromise format: `IPv4 Address`, `Domain / URL`, `File Hash (SHA256)`, `C2 Beacon Endpoint`. |
| `IOC_Value` | String | Dimension | The specific malicious artifact value. |
| `MTTD_Hours` | Real (Float) | Measure | Mean Time to Detect (in hours) by internal SOC or MDR sensors. |
| `MTTR_Hours` | Real (Float) | Measure | Mean Time to Respond & Remediate (in hours). |
| `Incident_Status` | String | Dimension | Containment status: `Blocked`, `Contained`, `Under Remediation`, `Resolved / Closed`. |
| `Financial_Impact_USD` | Integer | Measure | Direct and indirect monetary impact or damages mitigated in USD ($). |
| `Confidence_Score` | String | Dimension | Attribution confidence level: `High`, `Medium`, `Low`. |
| `TLP_Marking` | String | Dimension | Traffic Light Protocol classification: `TLP:CLEAR`, `TLP:GREEN`, `TLP:AMBER`, `TLP:AMBER+STRICT`, `TLP:RED`. |
