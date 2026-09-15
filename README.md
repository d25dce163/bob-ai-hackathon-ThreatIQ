# 🚀 ThreatIQ — Threat Intelligence Correlation & Alert Prioritisation Assistant

> **Turn Alert Noise into Actionable Intelligence.**

ThreatIQ is an AI-powered cybersecurity platform designed to help Security Operations Center (SOC) analysts process large volumes of security alerts, correlate related events, identify potential threats and false positives, prioritize incidents by risk, map attacker behavior to MITRE ATT&CK techniques, and generate concise AI-powered security summaries.

---

## 👥 Team

| Field         | Value                                                                          |
| ------------- | ------------------------------------------------------------------------------ |
| **Team Name** | ThreatIQ                                                                       |
| **Track**     | Open                                                                           |
| **Team Lead** | Sakshi Dhanani(D25DCE163)                                                      |
| **Members**   | Krisha Vegad (D25DCE162), Diksha Akbari (D25DCE153), Riddhi Pujara (D25DCS173) |

---

## 🎯 Problem Statement

Security teams receive a large number of alerts from different sources such as SIEM systems, IDS/IPS, endpoint security tools, firewalls, authentication systems, and threat-intelligence feeds. These alerts can be duplicated, noisy, unrelated, or difficult to investigate individually, making it challenging for SOC analysts to identify genuine threats and prioritize the most critical incidents.

The selected industry problem is **D2 — Threat Intelligence Correlation & Alert Prioritisation Assistant**. The goal is to correlate multi-source security alerts, distinguish potential genuine threats from false positives, map attacker behavior to MITRE ATT&CK techniques, and provide prioritized and explainable threat intelligence to security analysts.

---

## 💡 Solution

**ThreatIQ** is an AI-powered threat intelligence and alert prioritisation platform that transforms raw security alerts into actionable security incidents.

The platform normalizes incoming security events, correlates related alerts, identifies suspicious activity, calculates an explainable risk score, maps observed behavior to MITRE ATT&CK techniques, and generates an AI-powered **BLUF (Bottom Line Up Front)** summary with recommended investigation actions.

Instead of requiring analysts to manually investigate hundreds of individual alerts, ThreatIQ provides a centralized SOC-style dashboard that highlights the most important incidents first and explains why they deserve attention.

---

## ✨ Key Features

### 🔗 Intelligent Alert Correlation

Groups related alerts based on common indicators such as:

* Source IP
* Destination IP
* Host
* User
* Domain
* Timestamp
* Attack behavior
* Threat intelligence indicators

Multiple related alerts can be combined into a single security incident.

### 🎯 Explainable Threat Prioritisation

ThreatIQ assigns a risk score from **0–100** based on factors such as:

* Alert severity
* Confidence
* Asset criticality
* Threat intelligence matches
* Number of correlated alerts
* Attack behavior
* Recency
* Potential impact

The system also explains the factors contributing to the final risk score.

### 🛡️ False Positive Analysis

ThreatIQ identifies alerts that may be:

* Genuine threats
* Suspicious activity
* Likely false positives

Each classification is accompanied by an explanation where possible.

### 🧩 MITRE ATT&CK Mapping

Observed attacker behavior can be mapped to relevant MITRE ATT&CK techniques and tactics.

Examples include:

* T1003 — OS Credential Dumping
* T1059 — Command and Scripting Interpreter
* T1566 — Phishing
* T1071 — Application Layer Protocol

### 🤖 AI Threat Analysis

AI-assisted analysis provides:

* Threat explanations
* Incident summaries
* Correlation explanations
* Risk explanations
* Recommended investigation actions
* Threat intelligence interpretation

### ⚡ AI BLUF

ThreatIQ generates a concise **Bottom Line Up Front (BLUF)** summary for high-priority incidents.

The summary highlights:

* What happened
* Why it matters
* Risk level
* Related attack techniques
* Recommended actions

### 🧠 AI Security Copilot

Analysts can ask security-related questions such as:

* "What are today's most critical incidents?"
* "Why is this incident high risk?"
* "Which MITRE techniques were detected?"
* "Which alerts may be false positives?"
* "Summarize this incident."
* "What should the SOC investigate first?"

### 📊 SOC Dashboard

A centralized security dashboard provides:

* Total alerts
* Critical alerts
* Active incidents
* Risk scores
* False-positive statistics
* Alert trends
* Threat activity
* Top attack techniques
* Threat sources

### 🔍 Threat Intelligence

ThreatIQ can analyze indicators such as:

* IP addresses
* Domains
* URLs
* File hashes
* Other security indicators

Indicators can be associated with alerts and incidents to improve threat prioritisation.

### 🚨 Threat Simulation / Demo Mode

A predefined attack scenario can be used to demonstrate the complete ThreatIQ workflow:

**Security Alerts → Correlation → Incident → Risk Score → MITRE Mapping → AI Analysis → BLUF → Recommended Actions**

---

## 🛠️ Tech Stack

| Category               | Technologies                                         |
| ---------------------- | ---------------------------------------------------- |
| **Languages**          | Python, JavaScript / TypeScript                      |
| **Frontend**           | React, Vite                                          |
| **Backend**            | FastAPI / REST API                                   |
| **AI**                 | AI/LLM-based threat analysis                         |
| **Cybersecurity**      | MITRE ATT&CK, Threat Intelligence, Alert Correlation |
| **Database / Storage** | Project data storage / sample JSON or database layer |
| **Development**        | Git, GitHub                                          |
| **Hackathon Platform** | IBM BoB                                              |
| **Other**              | HTML, CSS, REST APIs                                 |

> The exact technology configuration may be updated according to the final implementation in the project repository.

---

## 🏗️ System Workflow

```text
┌───────────────────────────┐
│   Security Alert Sources  │
│ SIEM / IDS / Firewall /   │
│ Endpoint / Threat Feeds   │
└─────────────┬─────────────┘
              │
              ▼
┌───────────────────────────┐
│      Data Ingestion       │
└─────────────┬─────────────┘
              │
              ▼
┌───────────────────────────┐
│   Alert Normalization     │
└─────────────┬─────────────┘
              │
              ▼
┌───────────────────────────┐
│    Alert Correlation      │
└─────────────┬─────────────┘
              │
              ▼
┌───────────────────────────┐
│ Threat / False Positive   │
│        Analysis           │
└─────────────┬─────────────┘
              │
              ▼
┌───────────────────────────┐
│   Risk & Priority Score   │
└─────────────┬─────────────┘
              │
              ▼
┌───────────────────────────┐
│    MITRE ATT&CK Mapping   │
└─────────────┬─────────────┘
              │
              ▼
┌───────────────────────────┐
│       AI Analysis         │
│   BLUF + Recommendations  │
└─────────────┬─────────────┘
              │
              ▼
┌───────────────────────────┐
│       SOC Dashboard       │
└───────────────────────────┘
```

---

## 📁 Repository Structure

```text
bob-ai-hackathon-ThreatIQ/
│
├── frontend/                  # ThreatIQ web interface
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── layouts/
│   │   ├── services/
│   │   └── data/
│   └── ...
│
├── backend/                   # Backend services and APIs
│   ├── api/
│   ├── services/
│   ├── ai/
│   ├── correlation/
│   ├── detection/
│   ├── mitre/
│   └── ...
│
├── sample-data/               # Sample cybersecurity data
│   ├── alerts.json
│   ├── incidents.json
│   └── threat-intelligence.json
│
├── docs/                      # Project documentation
│   ├── problem-statement.md
│   ├── solution-overview.md
│   ├── architecture.md
│   └── setup-guide.md
│
├── demo/                      # Demonstration materials
│   ├── screenshots/
│   ├── demo-video-link.txt
│   └── live-demo-url.txt
│
├── presentation/              # Presentation materials
│
├── README.md
├── .env.example
└── submission.yaml
```

> The structure above represents the intended organization. Update it if the final implementation generated in the repository uses different folders.

---

## ⚡ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/<YOUR-GITHUB-USERNAME>/bob-ai-hackathon-ThreatIQ.git
cd bob-ai-hackathon-ThreatIQ
```

### 2. Install dependencies

Install the dependencies according to the frontend and backend setup.

For the frontend:

```bash
cd frontend
npm install
```

For the backend, follow the instructions provided in:

```text
docs/setup-guide.md
```

### 3. Configure environment variables

Create the environment file:

```bash
cp .env.example .env
```

Add the required configuration values.

**Never commit API keys or other secrets to GitHub.**

### 4. Start the application

Start the backend and frontend using the commands specified in:

```text
docs/setup-guide.md
```

The application can then be opened in the browser using the local URL displayed by the development server.

---

## 🖥️ Demo

| Artifact            | Link                                                                                   |
| ------------------- | -------------------------------------------------------------------------------------- |
| 📹 **Demo Video**   | [See ](demo/demo-video-link.txt)[`demo/demo-video-link.txt`](demo/demo-video-link.txt) |
| 🌐 **Live Demo**    | [See ](demo/live-demo-url.txt)[`demo/live-demo-url.txt`](demo/live-demo-url.txt)       |
| 🖼️ **Screenshots** | [See ](demo/screenshots/)[`demo/screenshots/`](demo/screenshots/)                      |
| 📊 **Presentation** | [See ](presentation/)[`presentation/`](presentation/)                                  |

> Demo links will be added when the final demo and deployment are available.

---

## 🎬 Recommended Demo Flow

The ThreatIQ demonstration follows a realistic SOC investigation:

```text
1. Open ThreatIQ Dashboard
            ↓
2. View incoming security alerts
            ↓
3. Filter Critical / High alerts
            ↓
4. Open a high-risk alert
            ↓
5. Correlate related alerts
            ↓
6. Generate security incident
            ↓
7. Calculate explainable risk score
            ↓
8. Map behavior to MITRE ATT&CK
            ↓
9. Generate AI BLUF
            ↓
10. View recommended actions
            ↓
11. Ask AI Security Copilot
```

---

## 📊 Example Threat Scenario

### Credential Compromise Scenario

ThreatIQ can demonstrate a multi-stage attack:

```text
Failed Login Attempts
        ↓
Successful Login
        ↓
Suspicious Authentication
        ↓
Credential Dumping
        ↓
Privilege Escalation
        ↓
Suspicious PowerShell Activity
        ↓
Possible Command & Control
```

ThreatIQ correlates these events and presents them as a single incident rather than requiring the analyst to investigate every alert independently.

Example result:

```text
Incident: INC-1024

Priority: CRITICAL
Risk Score: 91/100

Possible Techniques:
T1003 — OS Credential Dumping
T1059 — Command and Scripting Interpreter

Status:
Investigation Required
```

---

## 🔐 Security Considerations

ThreatIQ follows basic secure-development practices including:

* Environment variables for sensitive configuration
* No hardcoded API credentials
* Input validation
* API error handling
* Sanitization of user-provided data
* Separation of frontend and backend services
* Clear handling of unavailable AI services
* Explainable risk scoring

This project is a hackathon prototype and should not be considered a production-ready enterprise SOC platform without additional security hardening and testing.

---

## ⚠️ Known Limitations

* The project uses sample cybersecurity data for the hackathon demonstration.
* Live enterprise SIEM/IDS integrations may not be available in the prototype.
* Threat intelligence feeds may be simulated or limited depending on available APIs.
* AI-generated threat analysis may require an external AI service or configured model.
* AI recommendations should be reviewed by qualified security analysts before real-world action.
* Authentication and authorization may be simplified for the hackathon prototype.
* The current implementation is designed as a demonstration/MVP rather than a production enterprise SOC platform.
* Accuracy of threat classification and MITRE ATT&CK mapping depends on the available alert data and analysis logic.

---

## 🚀 Future Scope

Future versions of ThreatIQ could include:

* Integration with enterprise SIEM platforms
* Real-time threat intelligence feeds
* Automated IOC enrichment
* Advanced behavioral analytics
* Machine-learning-based anomaly detection
* Automated incident response workflows
* SOAR integration
* More comprehensive MITRE ATT&CK coverage
* Threat hunting capabilities
* Role-based access control
* Enterprise authentication
* Cloud deployment
* Historical threat analytics
* Automated threat-intelligence ingestion
* Continuous model evaluation

---

## 🏅 What We're Most Proud Of

We are most proud of **ThreatIQ's ability to reduce security-alert overload by turning multiple raw alerts into a prioritized and explainable security story**.

Instead of presenting a SOC analyst with a long list of disconnected alerts, ThreatIQ focuses attention on the incidents that matter most by correlating related events, assigning an explainable risk score, mapping attacker behavior to MITRE ATT&CK techniques, and generating an AI-powered BLUF summary with recommended investigation actions.

The project combines **cybersecurity, threat intelligence, AI-assisted analysis, explainability, and an intuitive SOC dashboard** into one practical solution for the D2 industry problem.

---

## 👥 Team

### ThreatIQ

| Name              | Student ID | Role        |
| ----------------- | ---------- | ----------- |
| **Krisha Vegad**  | D25DCE162  | Team Member |
| **Diksha Akbari** | D25DCE153  | Team Member |
| **Riddhi Pujara** | D25DCS173  | Team Member |

---

## 📌 Project Information

**Project:** ThreatIQ
**Problem:** D2 — Threat Intelligence Correlation & Alert Prioritisation Assistant
**Team:** ThreatIQ
**Hackathon:** IBM BoB AI Innovation Hackathon 2026
**Repository:** `bob-ai-hackathon-ThreatIQ`

---

## 📄 License

This project was developed as part of the **IBM BoB AI Innovation Hackathon 2026**.

The project is intended for educational, research, and hackathon demonstration purposes.
