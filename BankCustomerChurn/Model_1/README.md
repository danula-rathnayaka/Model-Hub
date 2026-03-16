# Bank Customer Churn Prediction

## Overview

This project builds a **Machine Learning model to predict bank customer churn** using a customer dataset.
Customer churn occurs when a customer stops using the bank’s services. Predicting churn helps banks identify customers who are likely to leave and take preventive actions.

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

The following steps were applied:

- Removed unnecessary columns
  - `RowNumber`
  - `CustomerId`
  - `Surname`

- Encoded categorical features
  - `Geography`
  - `Gender`

- Split the dataset
  - **80% Training**
  - **20% Testing**

- Applied **StandardScaler** for feature scaling

---

## Machine Learning Model

The model used in this project:

**Logistic Regression**

---

## Model Performance

| Metric   | Score    |
| -------- | -------- |
| Accuracy | **0.81** |

SMOTE was tested for class balancing but reduced the model performance, so the final model was trained **without SMOTE**.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn

---

---

## Project Goal

To build a machine learning model that predicts whether a bank customer will churn based on customer data.
