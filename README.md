# Customer_Churn_Analysis - telecom industry 
Predicting Telecom customer churn using machine learning models and extarcting buisness insights though a Power BI dashboard.

## 📌 Project Overview

Customer churn significantly impacts a company’s revenue. This project analyzes a telecom dataset to understand the key factors driving churn and builds machine learning models to predict customer exit. We also deliver actionable insights via a dashboard to help the business improve retention.

## 🧠 Problem Statement

> How can we predict which customers are likely to leave a telecom service based on usage, billing, and service features?

With over 7,000 customer records, this project builds a classification model to forecast churn and visually communicate patterns to business teams.

## 📊 Dataset Description

- **Source**: [Telco Customer Churn – Kaggle / UCI](https://www.kaggle.com/blastchar/telco-customer-churn)
- **Rows**: 7,043 customers
- **Columns**: 21
- **Target variable**: `Churn` (Yes/No)

| Column            | Description                          |
|-------------------|--------------------------------------|
| `gender`          | Male / Female                        |
| `SeniorCitizen`   | Binary (0 = No, 1 = Yes)             |
| `tenure`          | Months customer has stayed           |
| `Contract`        | Month-to-month / One year / Two year|
| `MonthlyCharges`  | Monthly bill amount                  |
| `TotalCharges`    | Total amount billed                  |
| ...               | Internet service, payment method, etc.|

## 🧹 Data Preprocessing & Cleaning

- Removed irrelevant columns (`customerID`)
- Handled missing / blank values
- Converted categorical columns using **Label Encoding**
- Converted `TotalCharges` to numeric
- Created train-test split (80-20)

## 📊 Exploratory Data Analysis (EDA)

Key findings:
- Customers with **month-to-month** contracts churn the most
- **Senior citizens** and **single customers** are more likely to churn
- Higher **monthly charges** relate to higher churn risk

EDA visuals included:
- Heatmaps
- Count plots
- Bar charts by churn & contract type

## 🤖 Machine Learning Models

Trained two models on the cleaned dataset:

| Model                | Accuracy  |
|----------------------|-----------|
| Logistic Regression  | ~80.4%    |
| Random Forest        | ~85.7% ✅ |

✅ **Random Forest** was selected based on performance.

Model evaluation metrics:
- Confusion Matrix
- Precision, Recall, F1-Score
- Feature importance plot

## 📈 Dashboard (Power BI)

An interactive dashboard was built using Power BI with:

- **KPI Cards**: Total Customers, Churn Rate
- **Bar Chart**: Churn by Contract Type
- **Pie Chart**: Payment Method Distribution
- **Line Chart**: Tenure vs Monthly Charges
- **Slicers**: Gender, Contract Type, Senior Citizen


