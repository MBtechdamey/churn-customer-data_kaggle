# Bank Customer Churn Prediction

A machine learning project that predicts whether a bank customer is likely to leave the bank (`Exited = 1`). The project compares multiple classification algorithms and investigates different techniques for handling class imbalance.

## Overview

Customer churn is an important business problem for banks, as identifying customers who are likely to leave can help organizations take proactive retention measures.

This project analyzes the **Churn Modelling** dataset and evaluates several machine learning models for predicting customer churn. Particular attention is given to the challenges of **imbalanced classification** and the use of resampling techniques such as **SMOTE** and **SMOTETomek**.

## Dataset

The dataset contains customer-level information including:

* Credit Score
* Geography
* Gender
* Age
* Tenure
* Balance
* Number of Products
* Credit Card Status
* Active Membership Status
* Estimated Salary

The target variable is:

* **Exited** — `1` if the customer exited the bank, otherwise `0`

## Machine Learning Models

The following classification algorithms are implemented and compared:

* Logistic Regression
* Polynomial Logistic Regression
* Support Vector Classifier (SVC)
* Decision Tree Classifier
* XGBoost
* Easy Ensemble Classifier

## Handling Class Imbalance

Because customer churn represents a minority class in the dataset, the project investigates resampling techniques to improve the model's ability to identify customers who are likely to churn.

The following approaches are explored:

* **SMOTE (Synthetic Minority Over-sampling Technique)**
* **SMOTETomek**

These techniques are compared with models trained on the original imbalanced dataset.

## Project Workflow

1. Data loading and cleaning
2. Exploratory Data Analysis (EDA)
3. Feature selection and preprocessing
4. Categorical feature encoding
5. Train/test splitting
6. Baseline model training
7. Class-imbalance handling
8. Model training with SMOTE and SMOTETomek
9. Model comparison
10. Performance evaluation

## Model Evaluation

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

Since the dataset is imbalanced, **precision, recall, F1-score, and the confusion matrix** are particularly important when assessing how effectively each model identifies customers who are likely to churn.

## Key Takeaway

This project demonstrates how different machine learning algorithms perform on a customer churn prediction problem and highlights the importance of addressing class imbalance.

Techniques such as **SMOTE** and **SMOTETomek** can help improve the detection of minority-class customers, providing potentially more useful predictions for customer retention strategies.

## Technologies

**Python • Pandas • NumPy • Scikit-learn • Imbalanced-learn • XGBoost • Matplotlib • Seaborn**

## Notebook

The complete data analysis, preprocessing, model training, resampling experiments, and evaluation are available in the Jupyter Notebook included in this repository.
