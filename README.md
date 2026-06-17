# Customer-Churn-Prediction-Pipeline

## Overview

This project develops an end-to-end machine learning pipeline for predicting customer churn using the Telco Customer Churn Dataset. The pipeline automates data preprocessing, model training, hyperparameter tuning, evaluation, and model export.

The objective is to identify customers who are likely to leave the telecom company so that retention strategies can be implemented.

---

## Objective

To build a production-ready machine learning pipeline using Scikit-Learn Pipeline API that predicts customer churn based on customer demographics, account information, and subscribed services.

---

## Dataset

Dataset: Telco Customer Churn Dataset

Target Variable:

* Churn = Yes (Customer Left)
* Churn = No (Customer Stayed)

Features include:

* Gender
* Senior Citizen
* Partner
* Dependents
* Tenure
* Internet Service
* Contract Type
* Monthly Charges
* Total Charges
* Payment Method
* Multiple additional customer attributes

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* Matplotlib
* Seaborn
* Joblib

---

## Methodology

### 1. Data Preprocessing

* Removed unnecessary columns
* Converted TotalCharges to numeric format
* Handled missing values
* Encoded categorical variables
* Scaled numerical features

### 2. Pipeline Construction

A reusable machine learning pipeline was created using:

* Pipeline
* ColumnTransformer
* SimpleImputer
* StandardScaler
* OneHotEncoder

### 3. Model Training

Two classification models were trained:

* Logistic Regression
* Random Forest Classifier

### 4. Hyperparameter Tuning

GridSearchCV was applied to optimize Random Forest parameters.

### 5. Model Evaluation

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

### 6. Model Export

The final pipeline was saved using Joblib for future deployment and reuse.

---

## Results

### Logistic Regression

* Accuracy: 82.11%
* Precision: 69%
* Recall: 60%
* F1-Score: 64%

### Random Forest

* Accuracy: 80.41%
* Precision: 67%
* Recall: 52%
* F1-Score: 58%

---

## Key Findings

* Logistic Regression achieved the best overall performance.
* Random Forest provided competitive results after hyperparameter tuning.
* The pipeline successfully automated preprocessing and prediction workflows.
* Exporting the model using Joblib improved deployment readiness.

---

## Business Impact

The developed model can help telecom companies:

* Identify customers at risk of leaving
* Improve customer retention
* Reduce revenue loss
* Support targeted marketing campaigns

---

## Future Improvements

* XGBoost
* LightGBM
* SMOTE for class balancing
* Feature Engineering
* Streamlit Deployment
* Real-Time Churn Prediction

---

## Author

Developed as part of the AI/ML Engineering Internship Program at DevelopersHub Corporation.
