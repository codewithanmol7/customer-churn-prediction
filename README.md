# Customer Churn Prediction — Machine Learning Web App

## Project Overview

Customer churn is one of the biggest challenges for subscription-based businesses. This project builds an end‑to‑end Machine Learning system that predicts whether a telecom customer is likely to churn based on demographic, service, and billing information.

The solution includes:

* Data preprocessing and feature engineering
* Class imbalance handling using SMOTE
* Model training using XGBoost
* Model evaluation with classification metrics
* Model serialization for deployment
* Interactive web application using Streamlit
* Cloud deployment for real-time predictions

This project demonstrates a complete production-style ML pipeline from raw data to deployed application.

---

## Live Demo

Streamlit App:

https://customer-churn-prediction-9btdyw4xwsnzvvdhvtsiuw.streamlit.app

GitHub Repository:

https://github.com/codewithanmol7/customer-churn-prediction
---

## Business Problem

Customer acquisition is expensive. Retaining existing customers is significantly more cost-effective. By predicting which customers are at risk of leaving, businesses can take proactive retention measures such as:

* Personalized offers
* Customer support intervention
* Contract restructuring
* Loyalty incentives

This model helps identify high-risk customers early.

---

## Dataset

Dataset: Telco Customer Churn

Features include:

* Customer demographics
* Service subscriptions
* Billing information
* Contract type
* Tenure
* Payment methods

Target variable:

* Churn (Yes / No)

---

## Machine Learning Pipeline

### 1. Data Cleaning

* Converted TotalCharges to numeric
* Handled missing values
* Encoded categorical variables

### 2. Feature Engineering

* Selected 19 predictive features
* Standardized numerical inputs where required

### 3. Class Imbalance Handling

* Applied SMOTE (Synthetic Minority Oversampling Technique)

### 4. Model Training

Algorithm used:

* XGBoost Classifier

Why XGBoost?

* High performance on tabular data
* Handles non-linear relationships
* Robust to feature interactions

### 5. Model Evaluation

Metrics used:

* Accuracy
* Precision
* Recall
* F1 Score

Test Accuracy: ~77%

### 6. Model Persistence

Saved using joblib:

* customer_churn_model.pkl
* churn_encoders.pkl

---

## Web Application (Streamlit)

The deployed app allows users to:

* Input customer details
* Generate churn prediction
* View model information
* Understand key predictors

Interface sections:

* Demographics
* Services
* Account information
* Prediction result

---

## Project Structure

```
customer-churn-prediction/
│
├── churn_app.py
├── customer.ipynb
├── customer_churn_model.pkl
├── churn_encoders.pkl
├── Telco-Customer-Churn.csv
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Installation (Local Setup)

### Clone repository

```
git clone https://github.com/codewithanmol7/customer-churn-prediction.git
cd customer-churn-prediction
```

### Create virtual environment (Mac M1)

```
python3 -m venv venv
source venv/bin/activate
```

### Install dependencies

```
pip install -r requirements.txt
```

### Run Streamlit app

```
streamlit run churn_app.py
```

---

## Technologies Used

Machine Learning

* Python
* Scikit-learn
* XGBoost
* Pandas
* NumPy

Visualization

* Matplotlib
* Seaborn
* Plotly

Deployment

* Streamlit
* GitHub

---

## Model Information

* Algorithm: XGBoost Classifier
* Training Samples: 7,000+
* Features: 19
* Class balancing: SMOTE
* Use case: Binary classification

---

## Key Predictors

Top features influencing churn:

* Contract type
* Tenure duration
* Monthly charges
* Internet service
* Payment method

---

## Evaluation Metrics 

```
Accuracy  : 0.77
Precision : 0.55
Recall    : 0.62
F1 Score  : 0.58
```

---

## Future Improvements

* SHAP explainability
* Hyperparameter tuning with GridSearch
* Docker containerization
* CI/CD deployment
* MLflow experiment tracking
* Probability-based risk scoring

---

## Resume Description (Use this)

Built an end-to-end machine learning system to predict telecom customer churn using XGBoost. Handled class imbalance with SMOTE, engineered predictive features, evaluated performance with classification metrics, and deployed an interactive Streamlit web application for real-time predictions.

---

## Author

Anmol Chaudhary

GitHub:
[https://github.com/codewithanmol7](https://github.com/codewithanmol7)

---

## License

This project is open-source and available for educational and research purposes.
