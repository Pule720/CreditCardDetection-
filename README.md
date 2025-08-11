# Credit Card Fraud Detection

## Project Overview
This project analyzes the [Kaggle Credit Card Fraud Detection dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud/data) to explore transaction patterns and build machine learning models to detect fraudulent transactions. The dataset is highly imbalanced, with fraud cases making up more or less than ~0.17% of total transactions.

## Contents
- **EDA (Exploratory Data Analysis)**
  - Class distribution (fraud vs legit)
  - Transaction amount and time distributions
  - Fraud vs legit amount comparison
  - Correlation heatmap of anonymized features
- **Modeling**
  - Logistic Regression
  - Random Forest
  - XGBoost with SMOTE for class balancing
- **Evaluation**
  - Precision-Recall AUC (PR AUC)
  - Final comparison of models

## Results
| Model                  | PR AUC  |
|------------------------|---------|
| Logistic Regression    | 0.7692  |
| Random Forest          | 0.8703  |
| XGBoost (SMOTE)        | 0.8761  |

As can be seen, I was able to achieve the best Precision Area Under the Curve (PR AUC) with XGBoost. 


- Tune hyperparameters with Genetic Algorithms
- Deploy the model as a real-time fraud detection API
