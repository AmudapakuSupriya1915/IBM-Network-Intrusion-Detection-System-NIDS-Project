# ⚔️ Network Intrusion Detection System (NIDS) using IBM watsonx.ai

A real-time machine learning solution designed to monitor, detect, classify, and analyze cybersecurity threats within network traffic using **IBM watsonx.ai**, **AutoAI**, and the **NSL-KDD dataset**. This project aims to support cybersecurity operations by providing automated intrusion detection through advanced supervised learning models.

## 📘 Overview
Cybersecurity threats are growing in complexity and frequency. Traditional firewalls and rule-based systems often struggle to detect zero-day and subtle multi-stage attacks. This project builds a **Network Intrusion Detection System (NIDS)** powered by machine learning to detect attacks with **high accuracy**, **low latency**, and **minimal false positives**.
Using the NSL-KDD dataset, we train models to classify network traffic as:
- 🟢 **Normal**  
- 🔥 **Denial of Service (DoS)**  
- 🔍 **Probe Attacks**  
- 🔐 **Remote to Local (R2L)**  
- 🧬 **User to Root (U2R)**  
This solution is deployed via IBM Cloud using **watsonx.ai**, with options for REST API integration into broader enterprise architectures.

## 🎯 Problem Statement
 **Goal:** Create a robust network intrusion detection system (NIDS) using machine learning. The system should be capable of analyzing network traffic data to identify and classify various types of cyber-attacks (e.g., DoS, Probe, R2L, U2R) and distinguish them from normal network activity. The goal is to build a model that can effectively secure communication networks by providing an early warning of malicious activities.

**Key Requirements: **
- High classification accuracy across all classes
- Effective handling of categorical and continuous features
- Minimal false positives to avoid alert fatigue
- Scalable deployment architecture (via IBM Cloud)

## 🔗 Dataset Information

- **Name:** NSL-KDD (Enhanced KDD'99)
- **Source:** [NSL-KDD Kaggle Dataset](https://www.kaggle.com/datasets/ghazouaniabdellatif/nslkdd)
- **Format:** CSV (`KDDTrain+`, `KDDTest+`)
- **Classes:**
  - `normal`
  - `dos`, `probe`, `r2l`, `u2r` (20+ attack subtypes)
- **Features:** 41 attributes (both categorical and numeric)

**Why NSL-KDD?**
- Removes duplicate entries from KDD'99
- Better balanced class distribution
- Better suited for modern ML evaluation

## 🧰 Technology Stack

| Layer            | Tool/Technology                             |
|------------------|---------------------------------------------|
| Platform         | IBM Watsonx.ai Studio                       |
| Development      | Jupyter Notebook, Python                    |
| ML Libraries     | scikit-learn, seaborn, pandas, matplotlib   |
| AutoML           | IBM AutoAI (GUI-based modeling)             |
| Cloud Deployment | IBM Cloud Lite, Watson ML Deployment        |
| Backend API      | RESTful Endpoint (via Watsonx pipeline)     |
| Visualization    | Seaborn, Matplotlib                         |
| Runtime Region   | Chennai (India), Sydney (Australia)         |


## 🧪 Core Features

- ✅ **multi-class classification**: Detects DoS, Probe, R2L, U2R, and Normal traffic
- 🔁 **Data preprocessing**:
  - One-hot encoding for categorical features
  - StandardScaler/MinMaxScaler for normalization
- 🎯 **Model Training**:
  - Manual tuning + AutoAI pipeline
  - Random Forest, Logistic Regression, Decision Tree, KNN
- 🧠 **Feature Importance**: Via Random Forest & AutoAI insights
- 📊 **Evaluation Metrics**:
  - Confusion Matrix, Precision, Recall, F1-Score, Accuracy
- ☁️ **Cloud Deployment**:
  - REST API access for integration with external systems
- 🔐 **Security Considerations**:
  - Model deployed within IBM Cloud secure zone
  - Dataset pre-sanitized to avoid leakage and bias

## 🚀 Step-by-Step Setup Instructions
```bash
1. Sign in to: https://cloud.ibm.com

2. Launch: IBM Watsonx.ai Studio → Create a New Project

3. Upload Files:
   - Dataset: KDDTrain+.csv, KDDTest+.csv
   - Notebook: intrusion-detection-nslkdd.ipynb

4. Choose Runtime:
   - Jupyter Notebook for manual ML pipeline
   - AutoAI for automated modeling

5. Run Preprocessing:
   - Labels encode & scale features

6. Train & Evaluate Models

7. Visualize Confusion Matrix & Feature Importance

8. Deploy Best Model:
   - Create Watson ML deployment
   - Expose as REST API

9. Test & Visualize:
   - Run sample API inference
   - Download classification reports

Metric	Value (Random Forest)
Accuracy	90% – 92%
Precision	High (90%+ for DoS)
Recall	High (esp. for Normal)
F1-Score	Balanced across classes
Note: Evaluation scores may vary based on feature selection, model tuning, and dataset balancing.

📈 Visualizations

•	✅ Confusion Matrix for each attack class
•	🔍 Classification Report Table
•	🌲 Feature Importance Bar Graph (Random Forest)
•	📊 AutoAI-generated Pipeline & Leaderboard

🧠 Future Enhancements
Feature	Description
🕵️ Real-time Packet Stream	Integrate PCAP (packet capture) feeds via scapy
🤖 Deep Learning Upgrade	Use CNN-LSTM hybrid for sequential traffic modeling
📊 Interactive Dashboard	Build a front-end with live alerts and stats
🔐 Encrypted Traffic Support	Integrate TLS/SSL packet parsing
🌐 Edge Deployment	Deploy lightweight model for routers/firewalls
📦 CI/CD Integration	GitHub Actions + IBM DevOps toolchain for deployment


🏆 Certifications & Acknowledgements
🎓 Certifications
•	IBM SkillsBuild – Watsonx.ai Agent Lab
•	IBM – AI Lifecycle & Deployment on IBM Cloud
•	Edunet Foundation – IBM skillbuild Internship
👨‍🏫 Mentorship & Support
•	IBM watsonx.ai Team
•	Edunet Foundation
•	NSL-KDD Dataset Authors

👩‍💻 Author Information
Supriya Amudapaku (Supriya.A)
🎓BCA, Sri Kanyaka Parameswari Arts and Science College for Women
💼 Python Developer Intern – Cybernaut Edu-Tech
📚 IBM SkillsBuild | Edunet Foundation
🔧 Tools: Python, AutoAI, scikit-learn, seaborn, IBM Watson

