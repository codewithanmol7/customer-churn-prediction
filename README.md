# Customer Churn Prediction (Machine Learning + Streamlit)

End-to-end machine learning project to predict telecom customer churn using behavioral and service usage data.  
The project includes data preprocessing, imbalance handling, model training with XGBoost, and a Streamlit web application for real-time predictions.


---

## Project Overview

Customer churn is a major challenge for subscription-based businesses.  
This project predicts whether a telecom customer is likely to leave the service based on demographics, account information, and service usage.

This helps businesses:
- Identify high-risk customers  
- Improve retention strategies  
- Reduce revenue loss  

---

## Features

- Data cleaning and preprocessing  
- Exploratory Data Analysis (EDA)  
- Class imbalance handling using SMOTE  
- XGBoost classification model  
- Model evaluation and performance metrics  
- Model serialization using joblib  
- Interactive Streamlit web application  
- GitHub-ready professional structure  

---

## Dataset

**Telco Customer Churn Dataset**

Contains customer information such as:

- Demographics (gender, senior citizen, dependents)
- Account details (tenure, contract type, payment method)
- Service subscriptions (internet, phone, streaming)
- Billing information (monthly charges, total charges)
- Target variable: `Churn`

---

## Machine Learning Pipeline

1. Data cleaning and missing value handling  
2. Encoding categorical features  
3. Train-test split  
4. Class imbalance correction (SMOTE)  
5. Model training using XGBoost  
6. Model evaluation (accuracy, confusion matrix, classification report)  
7. Model saving (`.pkl` files)  
8. Streamlit deployment for predictions  

---

## Model Used

### XGBoost Classifier

Why XGBoost:

- High performance on structured data  
- Handles non-linear relationships  
- Works well with imbalanced datasets  
- Provides feature importance  

---

## Model Performance 

| Metric | Score |
|------|------|
| Accuracy | XX% |
| Precision | XX% |
| Recall | XX% |
| F1 Score | XX% |

---

## Project Structure
customer-churn-prediction/
│
├── churn_app.py
├── customer.ipynb
├── requirements.txt
├── Telco-Customer-Churn.csv
├── .gitignore
└── README.md


### Folder Description

| Folder | Purpose |
|---|---|
| data | Contains raw dataset |
| notebooks | Model training, EDA, experimentation |
| models | Saved trained model and encoders |
| app | Streamlit deployment code |
| screenshots | Images used in README |
| root files | Config, dependencies, documentation |

---

## Recommended Professional Workflow

1. Load data from `/data`
2. Train model in `/notebooks`
3. Save model to `/models`
4. Use model in `/app` Streamlit interface
5. Document everything in README

---
