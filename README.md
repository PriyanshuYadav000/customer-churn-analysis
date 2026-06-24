# Customer Churn Prediction & Analysis

## Overview

Customer churn is one of the most important business challenges in subscription-based industries. Retaining existing customers is often more cost-effective than acquiring new ones.

This project analyzes customer behavior and develops a machine learning model to identify customers at risk of churn using the IBM Telco Customer Churn dataset.

---

## Dataset

Source: IBM Telco Customer Churn Dataset

Records: 7,032 customers

Features include:

* Customer demographics
* Account information
* Contract details
* Internet services
* Support services
* Billing information
* Churn status

---

## Project Workflow

### 1. Data Cleaning & Preparation

* Removed duplicate records
* Handled missing values in TotalCharges
* Converted data types
* Performed data quality checks

### 2. Exploratory Data Analysis

Analyzed churn behavior across:

* Contract types
* Customer tenure
* Monthly charges
* Internet services
* Online security
* Technical support

### 3. Feature Engineering

* Removed customer identifiers
* Encoded target variable
* Applied one-hot encoding
* Created training and testing datasets

### 4. Model Development

Built a Logistic Regression model using Scikit-Learn for churn prediction.

### 5. Model Interpretation

Analyzed feature coefficients to identify major churn drivers and retention factors.

---

## Model Performance

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 80.45% |
| Precision | 65.05% |
| Recall    | 57.22% |
| F1 Score  | 60.88% |

---

## Key Findings

* Month-to-month customers exhibit higher churn risk.
* Customers with shorter tenure are more likely to churn.
* Support-related services are associated with stronger retention.
* Contract type is one of the strongest predictors of churn behavior.

---

## Business Recommendations

* Encourage migration to long-term contracts.
* Improve onboarding for new customers.
* Promote support-related service adoption.
* Prioritize retention campaigns for high-risk customer segments.

---

## Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-Learn
* Jupyter Notebook

---

## Project Structure

customer-churn-analysis/

├── data/

│ ├── raw/

│ └── processed/

├── notebooks/

│ ├── 01_data_loading_eda.ipynb

│ ├── 02_feature_engineering_preprocessing.ipynb

│ ├── 03_logistic_regression_model.ipynb

│ └── 04_model_interpretation_business_insights.ipynb

├── README.md

├── requirements.txt

└── .gitignore
