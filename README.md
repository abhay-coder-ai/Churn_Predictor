# 🏦 Customer Churn Prediction – End-to-End ML Project

🚀 **Live App:**  
👉 https://churnxgboost.streamlit.app/

---

## 📌 Project Overview

Customer churn is a critical business problem where companies lose customers to competitors.  
This project builds an end-to-end Machine Learning pipeline to predict whether a customer will churn based on demographic and financial features.

The final deployed model uses **XGBoost**, selected after comparing multiple models.

---

## 🎯 Business Objective

- Identify customers likely to churn
- Enable targeted retention strategies
- Reduce customer acquisition cost
- Improve long-term revenue

---

## 📊 Dataset Information

- Total Records: 10,000
- Target Variable: `Churn` (0 = No, 1 = Yes)
- Class Distribution: ~80% Non-Churn, ~20% Churn
- Features:
  - Credit Score
  - Geography
  - Gender
  - Age
  - Tenure
  - Balance
  - Number of Products
  - Has Credit Card
  - Is Active Member
  - Estimated Salary

---

## 🔍 Exploratory Data Analysis (EDA)

- Identified class imbalance
- Analyzed feature distributions
- Detected and handled outliers using IQR
- Correlation analysis performed
- Key insights:
  - Germany showed higher churn rate
  - Inactive members churn more
  - Age positively correlates with churn

---

## 🧹 Data Preprocessing

- Removed duplicates
- OneHotEncoded categorical features:
  - Geography
  - Gender
- Applied StandardScaler (for distance-based models)
- Used Stratified Train-Test Split (80-20)
- Handled class imbalance using:
  - `class_weight`
  - `scale_pos_weight` in XGBoost

---

## 🤖 Models Implemented

The following models were trained and compared:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Support Vector Classifier (SVC)
- Decision Tree
- Random Forest
- XGBoost

Evaluation Metrics Used:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

---

## 🏆 Final Model Selection

**Selected Model: XGBoost**

Reasons:
- Highest Recall (best churn detection)
- Strong F1 Score
- Balanced performance
- Controlled overfitting

---

## 🖥 Deployment

The final model was deployed using:

- Streamlit (Frontend + Backend)
- XGBoost model serialized using Pickle
- Hosted on Streamlit Cloud

🔗 **Live App:**  
https://churnxgboost.streamlit.app/

---


