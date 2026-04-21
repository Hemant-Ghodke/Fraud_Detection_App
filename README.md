# 🚨 Fraud Detection App using Machine Learning

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-black?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-blue?logo=numpy)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?logo=scikitlearn)
![Streamlit](https://img.shields.io/badge/Streamlit-Web%20App-red?logo=streamlit)
![Model](https://img.shields.io/badge/Model-Logistic%20Regression-green)
![Accuracy](https://img.shields.io/badge/Accuracy-94.5%25-brightgreen)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Overview

This project is a **real-time Fraud Detection System** built using Machine Learning to identify fraudulent financial transactions.

It leverages a large-scale dataset (~6.3 million transactions) and achieves an accuracy of **94.5%** using Logistic Regression.

The system is deployed as an interactive web app using **Streamlit**, allowing users to input transaction details and instantly detect fraud.

---

## 🎯 Problem Statement

Financial fraud is a major challenge in digital transactions. Traditional systems often fail to detect fraud in real-time.

This project aims to:
- Detect fraudulent transactions accurately
- Provide real-time prediction capability
- Assist in preventing financial losses

---

## 📂 Dataset

- **Source:** Kaggle  
- **Dataset Name:** Fraud Detection Dataset  
- **Link:** https://www.kaggle.com/datasets/amanalisiddiqui/fraud-detection-dataset  
- **Records:** ~6.3 Million transactions  

### 🔑 Features

| Feature | Description |
|--------|------------|
| step | Time step of transaction |
| type | Type of transaction (PAYMENT, TRANSFER, etc.) |
| amount | Transaction amount |
| oldbalanceOrg | Sender balance before transaction |
| newbalanceOrig | Sender balance after transaction |
| oldbalanceDest | Receiver balance before |
| newbalanceDest | Receiver balance after |
| isFraud | Target variable (0 = Not Fraud, 1 = Fraud) |

---

## ⚙️ Tech Stack

- **Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  
- **Model:** Logistic Regression  
- **Frontend:** Streamlit  
- **Model Saving:** Joblib  

---

## 🧠 Machine Learning Model

### Model Used:
**Logistic Regression**

### Why Logistic Regression?
- Efficient for large datasets  
- Performs well for binary classification  
- Easy to interpret  

### 📊 Performance

- **Accuracy:** 94.5%  
- **Recall (Fraud Detection):** High (captures most fraud cases)  
- **Confusion Matrix:**  
  - True Positives: 2308  
  - False Negatives: 156  

---

## 🔄 Project Workflow

1. Data Loading  
2. Exploratory Data Analysis (EDA)  
3. Data Cleaning  
4. Feature Selection  
5. Encoding Categorical Variables  
6. Feature Scaling (StandardScaler)  
7. Train-Test Split  
8. Model Training (Logistic Regression)  
9. Model Evaluation  
10. Model Saving using Joblib  
11. Deployment using Streamlit  

---

## 📊 Exploratory Data Analysis (EDA)

Performed analysis to understand:

- Transaction types distribution  
- Fraud rate by transaction type  
- Transaction amount distribution  
- Fraud trends over time  
- Correlation between features  

### Key Insights:
- Fraud is highly imbalanced (~0.1%)  
- Most fraud occurs in **TRANSFER & CASH_OUT**  
- High-value transactions show higher fraud probability  

---

## 🚀 Features of the App

- ✅ Real-time fraud prediction  
- ✅ User-friendly interface (Streamlit)  
- ✅ Input-based transaction analysis  
- ✅ Instant classification (Fraud / Not Fraud)  
- ✅ Lightweight and fast  

---

## 🖥️ Streamlit App

### Input Fields:
- Transaction Type  
- Amount  
- Sender Balance (Before & After)  
- Receiver Balance (Before & After)  

### Output:
- Fraud Prediction (0 / 1)
- Alert message:
  - 🚨 Fraud detected
  - ✅ Safe transaction  

---

## 📁 Project Structure
Fraud-Detection-App/
│
├── AIML Dataset.csv
├── FraudDetection.ipynb
├── fraud_detection_pipeline.pkl
├── fraud_detection.py
└── README.md


---

## ▶️ How to Run the Project

### 1️⃣ Install Dependencies
pip install pandas numpy matplotlib seaborn scikit-learn streamlit

### 2️⃣ Run the App
streamlit run fraud_detection.py

---

## 📈 Key Insights

- Fraud transactions are extremely rare (high class imbalance)
- Certain transaction types are more vulnerable
- Balance differences play a critical role in fraud detection
- Logistic Regression performs well with proper preprocessing

---

## ⚠️ Limitations

- Dataset is highly imbalanced
- Low precision for fraud class (many false positives)
- Logistic Regression may not capture complex patterns

---

## 🔮 Future Improvements

- Use advanced models (Random Forest, XGBoost, Neural Networks)
- Handle class imbalance using SMOTE
- Deploy as API (Flask/FastAPI)
- Add real-time transaction streaming
- Improve UI/UX

---

## 📌 Conclusion

This project demonstrates how Machine Learning can be applied to detect fraud in financial transactions.

It combines:
- Data analysis  
- Machine learning  
- Real-time prediction  
- Web deployment  

to build a complete end-to-end intelligent system.

---

## 👨‍💻 Author

**Hemant Ghodke**  
Aspiring Data & Software Engineer  

---

## ⭐ If you like this project

Give it a ⭐ on GitHub and connect with me on LinkedIn!
