# Bank Customer Churn Prediction (XGBoost)

## Overview

This project builds a **Machine Learning model to predict bank customer churn** using the Bank Customer Churn dataset.

Customer churn occurs when a customer stops using the bank’s services. Predicting churn helps banks identify customers who are likely to leave and take preventive actions to retain them.

---

## Dataset

The dataset contains information about **10,000 bank customers**.

### Target Variable

- **Exited**
  - `1` → Customer left the bank
  - `0` → Customer stayed with the bank

### Target Distribution

- 0 (Stayed): **79.63%**
- 1 (Exited): **20.37%**

---

## Data Preprocessing

The following preprocessing steps were applied:

- Removed unnecessary columns
  - `CustomerId`
  - `Surname`

- Encoded categorical variables
  - `Geography`
  - `Gender`

- Split dataset into
  - **80% Training**
  - **20% Testing**

- Applied **StandardScaler** for feature scaling

---

## Machine Learning Model

The model used in this project:

**XGBoost Classifier**

XGBoost was chosen because it:

- Performs well on structured datasets
- Handles feature interactions effectively
- Often provides higher accuracy than traditional models

---

## Model Performance

| Metric   | Score     |
| -------- | --------- |
| Accuracy | **~0.87** |

The XGBoost model improved performance compared to simpler models such as Logistic Regression.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost

---

---

## Project Goal

The goal of this project is to develop a machine learning model that predicts whether a customer will churn based on banking data. This can help financial institutions take proactive steps to improve customer retention.
