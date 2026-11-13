\# SentinelX — AI-Powered Security Operations \& Threat Detection Platform



SentinelX is an AI-assisted Security Operations platform designed to analyze suspicious Indicators of Compromise (IOCs), detect potential threats, calculate risk, generate explainable security decisions, and manage security incidents through a SOC-style dashboard.



\## 🚀 Key Features



\- 🔎 Multi-IOC security scanner

\- 🤖 Machine Learning-based URL threat detection

\- 🛡️ Rule-based threat detection engine

\- 🧠 Hybrid AI + rule-based risk scoring

\- 📊 Risk score from 0–100

\- 🚦 ALLOW / ALERT / BLOCK decisions

\- 🔴 LOW / MEDIUM / HIGH / CRITICAL severity

\- 🔐 Trusted-domain protection

\- 🌐 Local threat intelligence

\- 📝 Explainable security analysis

\- 🚨 Automated incident creation

\- 📋 Incident management and status tracking

\- 📜 Scan history

\- 📈 SOC analytics dashboard

\- 🧪 ML model evaluation and metrics



\## 🏗️ Architecture



```text

Security Analyst

&#x20;      │

&#x20;      ▼

&#x20;  IOC / URL Input

&#x20;      │

&#x20;      ▼

┌───────────────────────┐

│ Detection Engine      │

│ Rule-Based Analysis   │

└──────────┬────────────┘

&#x20;          │

&#x20;          ▼

┌───────────────────────┐

│ ML Threat Detection   │

│ Random Forest Model   │

└──────────┬────────────┘

&#x20;          │

&#x20;          ▼

┌───────────────────────┐

│ Hybrid Risk Engine    │

│ Rules + ML + Context  │

└──────────┬────────────┘

&#x20;          │

&#x20;          ▼

┌───────────────────────┐

│ Explainability        │

│ Threat Intelligence   │

└──────────┬────────────┘

&#x20;          │

&#x20;          ▼

┌───────────────────────┐

│ Incident Management   │

└──────────┬────────────┘

&#x20;          │

&#x20;          ▼

&#x20;     SOC Dashboard

```



\## 🤖 Machine Learning



SentinelX uses a Random Forest classifier for URL threat detection.



\### Dataset



\- Total training dataset: \*\*60,030 URLs\*\*

\- Benign URLs: \*\*30,030\*\*

\- Malicious URLs: \*\*30,000\*\*

\- Extracted features: \*\*17\*\*



\### Model Performance



| Metric | Score |

|---|---:|

| Accuracy | 87.31% |

| Precision | 87.49% |

| Recall | 87.07% |

| F1 Score | 87.28% |

| ROC-AUC | 94.28% |



The ML model is used as one component of the overall detection pipeline rather than as the sole security decision-maker.



\## 🛡️ Hybrid Detection



SentinelX combines multiple security signals:



```text

Rule Detection

&#x20;     +

Machine Learning

&#x20;     +

Trusted Domain Context

&#x20;     +

Threat Intelligence

&#x20;     ↓

Hybrid Risk Score

&#x20;     ↓

Security Decision

```



\### Decision Logic



| Risk Score | Decision |

|---:|---|

| 0–29 | ALLOW |

| 30–79 | ALERT |

| 80–100 | BLOCK |



\### Severity



| Risk Score | Severity |

|---:|---|

| 0–29 | LOW |

| 30–59 | MEDIUM |

| 60–79 | HIGH |

| 80–100 | CRITICAL |



\## 📁 Project Structure



```text

SentinelX/

│

├── app.py

├── scan\_history.py

├──

├── engine/

│   ├── detector.py

│   ├── risk\_engine.py

│   ├── explainability.py

│   ├── threat\_intelligence.py

│   └── trusted\_domains.py

│

├── incidents/

│   └── incident\_manager.py

│

├── data/

│   └── threats.json

│

├── ml/

│   ├── feature\_extractor.py

│   ├── predictor.py

│   ├── train\_model.py

│   ├── prepare\_dataset.py

│   ├── dataset.csv

│   ├── dataset\_public.csv

│   ├── trusted\_benign.csv

│   └── model\_metrics.json

│

├── templates/

│   ├── dashboard.html

│   ├── scanner.html

│   ├── history.html

│   └── incidents.html

│

├── static/

│   ├── css/

│   └── js/

│

└── README.md

```



\## ⚙️ Technology Stack



\- \*\*Python\*\*

\- \*\*Flask\*\*

\- \*\*Scikit-learn\*\*

\- \*\*Pandas\*\*

\- \*\*NumPy\*\*

\- \*\*Joblib\*\*

\- \*\*HTML / CSS / JavaScript\*\*

\- \*\*JSON\*\*

\- \*\*Git / GitHub\*\*



\## ▶️ Running SentinelX



\### 1. Clone the repository



```bash

git clone https://github.com/bhaveshupadhyay2007-dev/SentinelX-AI-Security-Operations-Platform.git

cd SentinelX-AI-Security-Operations-Platform

```



\### 2. Create and activate a virtual environment



Windows:



```powershell

python -m venv venv

venv\\Scripts\\activate

```



\### 3. Install dependencies



```powershell

pip install flask pandas numpy scikit-learn joblib requests python-dotenv

```



\### 4. Start the application



```powershell

python app.py

```



Then open:



```text

http://127.0.0.1:5000

```



\## 🔬 Example Analysis



Example suspicious URL:



```text

http://verify-account-login.top/password

```



SentinelX can identify indicators such as:



\- Suspicious authentication keywords

\- Insecure HTTP connection

\- Suspicious top-level domain

\- Elevated risk score

\- Security severity

\- Recommended security decision

\- Incident generation



\## ⚠️ Security Note



SentinelX is an academic and portfolio-oriented security operations prototype.



The ML model and detection rules should not be treated as a replacement for production-grade threat intelligence, commercial security products, or human security analysts.



Detection results should be validated before taking real-world security actions.



\## 🎯 Project Goals



SentinelX was developed to demonstrate practical concepts in:



\- Cybersecurity

\- Security Operations Centers (SOC)

\- Threat Detection

\- Machine Learning

\- Risk Assessment

\- Threat Intelligence

\- Incident Management

\- Security Automation

\- Explainable Security Decisions



\## 👨‍💻 Project Status



\*\*Status: MVP / Portfolio Ready\*\*



The project currently contains an integrated security detection pipeline with machine learning, rule-based detection, risk scoring, threat intelligence, incident management, analytics, and a SOC-style web dashboard.


## Contributors
* **Saanvi** ([@saanvi0712](https://github.com))
* **Bhavesh Upadhyay** ([@bhaveshupadhyay2007-dev](https://github.com))


\---



\*\*SentinelX — Detect. Analyze. Respond.\*\*

