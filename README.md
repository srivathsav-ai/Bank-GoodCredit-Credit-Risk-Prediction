# Bank GoodCredit – Credit Risk Prediction

## 1. Project Overview

This project focuses on predicting and ranking bank customers based on their likelihood of becoming 30 or more days past due (30+ DPD).

The objective is to develop a machine learning-based credit risk prediction model that helps identify high-risk customers and supports data-driven credit risk management.

## 2. Problem Statement

Financial institutions need to identify customers who are more likely to default on their credit obligations.

This project uses historical customer account, payment history, and financial information to distinguish between good-credit and bad-credit customers and generate risk rankings.

## 3. Dataset Overview

* Total Customers: 23,896
* Total Account Records: 186,329
* Target Variable: `Bad_label`
* Good Credit Class: 0
* Bad Credit Class: 1
* Minority Class: Approximately 4.2%

The dataset contains customer-level information derived from account, demographic, enquiry, and payment-history records.

**Note:** Original client data is not included in this repository due to confidentiality considerations.

## 4. Technologies Used

* Python
* Pandas
* NumPy
* MySQL
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

## 5. Project Workflow

1. Data extraction and consolidation using MySQL.
2. Data cleaning and preprocessing.
3. Exploratory Data Analysis (EDA).
4. Customer-level feature engineering.
5. Handling class imbalance.
6. Model development and comparison.
7. Hyperparameter tuning.
8. Model evaluation using ROC-AUC and Gini.
9. Risk ranking and business recommendations.

## 6. Machine Learning Models

The following ensemble learning algorithms were evaluated:

* Random Forest
* AdaBoost
* Gradient Boosting

The tuned AdaBoost model achieved the best reported performance.

## 7. Model Performance

| Evaluation Metric     | Result |
| --------------------- | -----: |
| ROC-AUC               |  0.689 |
| Gini Coefficient      |   37.8 |
| Client Benchmark Gini |   37.9 |

## 8. Risk Ranking Results

The model demonstrated useful risk differentiation:

* Highest-risk 10% of customers: 10.7% bad rate.
* Lowest-risk 10% of customers: 1.0% bad rate.
* Highest-risk 20% accounted for approximately 45% of all bad customers.

These findings demonstrate the model's ability to prioritize customers based on predicted credit risk.

## 9. Business Recommendations

The developed risk score can support customer risk prioritization and help financial institutions establish appropriate decision thresholds based on their risk appetite.

## 10. Key Learnings

* Working with relational customer data using MySQL.
* Performing exploratory data analysis and data preprocessing.
* Engineering customer-level features.
* Handling imbalanced classification problems.
* Comparing and evaluating ensemble machine learning models.
* Interpreting model performance using Gini and ROC-AUC.
* Translating analytical results into business recommendations.

## 11. Project Files

The repository contains the Jupyter Notebook documenting the project workflow, analysis, model development, and evaluation.
