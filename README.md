# Fraud_detection_system_usingML
Fraud detection system built using Python, pandas, scikit-learn, and machine learning models to identify suspicious transaction
# 💳 Fraud Detection System

## 📌 Project Overview
This project implements a **Fraud Detection System** using machine learning.  
It analyzes financial transaction data, explores patterns, and trains a **Logistic Regression** model to classify transactions as **fraudulent** or **legitimate**.  

A **Streamlit web app** is included, where users can input transaction details and get instant fraud predictions.

---

## 📂 Dataset
- **Source:** `dataset/AIML Dataset.csv`(from kaggle)  
- **Features used:**
  - `type` → transaction type (PAYMENT, TRANSFER, CASH_OUT, DEPOSIT)  
  - `amount` → transaction amount  
  - `oldbalanceOrg`, `newbalanceOrig` → sender balances  
  - `oldbalanceDest`, `newbalanceDest` → receiver balances  
- **Target variable:**  
  - `isFraud` → `1` if fraud, `0` otherwise  

---

## 🔎 Exploratory Data Analysis (EDA)
- Checked missing values and dataset shape  
- Visualized distribution of transaction types  
- Analyzed correlation between features and fraud probability  
- Observed fraud is highly concentrated in **TRANSFER** and **CASH_OUT** transactions  
- Detected class imbalance (fraud cases are much fewer than legitimate ones)  

---

## 🧠 Machine Learning Pipeline
1. **Data Preprocessing**
   - Encoded categorical features (`type`)
   - Normalized numerical values (amount, balances)
   - Handled imbalanced data

2. **Model Training**
   - Algorithm: **Logistic Regression**
   - Dataset split: 70% training / 30% testing

3. **Evaluation Metrics**
   - Accuracy, Precision, Recall, F1-score  
   - Confusion Matrix to evaluate fraud detection performance

---

## 📊 Results
- Logistic Regression achieved:  
  - **Accuracy:** ~95%  
  - **Precision (Fraud):** High (low false positives)  
  - **Recall (Fraud):** Lower (frauds are rare → harder to catch)  

- Conclusion: Model works well but can be improved using advanced ML/DL techniques like **Random Forest, XGBoost, Neural Networks**.

---

## ⚙️ Installation

Clone the repository:
```bash
git clone https://github.com/naman12072000//Fraud_detection_system_usingML.git
cd Fraud_detection_system_usingML
```



## 🚀 Running the Streamlit App

Run the app:
```bash
streamlit run fraud_detection.py
```

Enter transaction details in the web app form and get a **fraud prediction instantly**.

---
fraud-detection-system/
│── dataset/
│   └── AIML Dataset.csv
│── fraud_detection.ipynb        # EDA + model training
│── fraud_detection_pipeline.pkl # saved ML model
│── fraud_detection.py                       # Streamlit app

│── README.md

## 📌 Future Improvements
- Use advanced models (Random Forest, XGBoost, Deep Learning)  
- Handle extreme class imbalance with **SMOTE** or anomaly detection  
- Deploy app on **Heroku/Streamlit Cloud/AWS**  
- Add real-time transaction monitoring  

---

## 👨‍💻 Author
Developed by *Naman Nirbhay*  
📧 Contact: n.nirbhaya@iitg.ac.in  


