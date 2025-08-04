# ⚔️ Network Intrusion Detection System (NIDS) - IBM watsonx.ai

    A machine learning solution to detect, classify, and analyze cybersecurity threats in real-time network traffic. This project leverages supervised learning techniques to monitor packets and identify potential intrusions.

    ## 📚 **Problem Statement**
    Design a robust Network Intrusion Detection System (NIDS) that classifies network connections into *normal* or various *attack types* (e.g., DoS, Probe, R2L, U2R). The system must handle categorical and continuous features efficiently to ensure high accuracy and low false positives.

    ## 🔗 **Dataset**
    **Kaggle**: [KDD Cup 99 / NSL-KDD Dataset](https://www.kaggle.com/datasets/ghazouaniabdellatif/nslkdd)
(Used sample of pre-processed Train and Test splits)

    ## 🛠️ **Technology Stack**
    - Platform: IBM watsonx.ai Studio
    - Runtime: watsonx.ai + IBM Granite Model
    - Modeling: Jupyter Notebooks (manual + AutoAI integration)
    - Deployment: IBM Cloud Lite
    - Tools Used: watsonx.ai Agent Lab, AutoAI, Watson Pipelines
    - Regions: Chennai and Sydney Datacenter

    ## 🧪 **Features**
    - Attack type classification (DoS, Probe, R2L, U2R, Normal)
    - Label encoding and feature scaling pipeline
    - Confusion matrix and performance visualizations
    - Feature importance analysis using Random Forest
    - Secure model deployment via IBM Cloud
    - AutoAI pipeline integration with tunable hyperparameters
    - Train/test split with robust evaluation metrics

    ## 🚀 **Setup Instructions**
    1. Login to IBM Cloud
    2. Open **watsonx.ai Studio** → Create New Project
    3. Upload CSV datasets and Jupyter Notebook
    4. Use AutoAI or manual ML pipeline to train and evaluate
    5. Deploy model and connect REST API endpoint for inference
    6. Visualize metrics and download reports

    ## 🏆** Certifications**
    - IBM SkillsBuild: watsonx.ai Agent Lab
    - IBM AI Lifecycle & Deployment on Cloud
    - Cybersecurity Internship Completion Certificate

    ## 🧠 **Future Enhancements**
    - Real-time packet capture integration
    - Deep learning model upgrade (CNN-LSTM)
    - Web-based intrusion alert dashboard
    - Encrypted traffic analysis support
   
    ## 👩‍💻 **Credits**
    Supriya Amudapaku, BCA – Sri Kanyaka Parameswari Arts and Science College  
    Internship: Cybernaut Programming Intern | IBM SkillsBuild | Edunet Foundation  
    Tools Used: Python, IBM Watson, watsonx.ai, AutoAI, sklearn, seaborn
