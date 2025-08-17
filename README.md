# Fraud_detection_system_usingML
Fraud detection system built using Python, pandas, scikit-learn, and machine learning models to identify suspicious transaction
# 💳 Fraud Detection System

## 📌 Project Overview
This project implements a **Fraud Detection System** using machine learning.  
It analyzes financial transaction data, explores patterns, and trains a **Logistic Regression** model to classify transactions as **fraudulent** or **legitimate**.  

A **Streamlit web app** is included, where users can input transaction details and get instant fraud predictions.

---

## 📂 Dataset
- **Source:** `dataset/AIML Dataset.csv from kaggel`  
- **Features used:**
  - `type` → transaction type (PAYMENT, TRANSFER, CASH_OUT, DEPOSIT)  
  - `amount` → transaction amount  
  - `oldbalanceOrg`, `newbalanceOrig` → sender balances  
  - `oldbalanceDest`, `newbalanceDest` → receiver balances  
- **Target variable:**  
  - `isFraud` → `1` if fraud, `0` otherwise  

---

## ⚙️ Installation

Clone the repository:
```bash
git clone https://github.com/your-username/fraud-detection-system.git
cd fraud-detection-system

