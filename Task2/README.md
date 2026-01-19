# Core ML Foundations (4 Parts)

## Dataset Source
- **Name:** Bank Marketing Dataset  
- **Source:** UCI Machine Learning Repository  
- **Description:**  
  The dataset contains information about customers contacted during a bank’s direct marketing campaigns.  
  The goal is to analyze customer attributes and predict whether a client will subscribe to a term deposit.  

---

## Problem Statement
The objective of this project is to:
1. Build a **machine learning pipeline**.
2. Implement:
   - **One supervised learning algorithm** (Logistic Regression)  
   - **One unsupervised learning algorithm** (K-Means Clustering)
3. Analyze and evaluate model behavior using appropriate metrics and visualizations.

Specifically:
- **Supervised task:** Binary classification to predict whether a customer will subscribe to a term deposit.  
- **Unsupervised task:** Customer segmentation using clustering to uncover hidden structure in the data.

---

## Execution Steps

### 1. Data Selection & Understanding
- Selected a real-world banking dataset.
- Identified relevant features:
  - `age`, `job`, `marital`, `default`, `balance`, `loan`, `housing`, `poutcome`
- Excluded `duration` to avoid data leakage.

### 2. Preprocessing
- Ordinal encoded binary variables.
- One-hot encoded nominal categorical variables.
- Applied Robust Scaling to numeric features to reduce the effect of outliers.
- Implemented a custom train_test_split with stratification.

### 3. Supervised Learning (From Scratch)
- Implemented **Logistic Regression from scratch** using:
  - Sigmoid function
  - Binary cross-entropy loss
  - Gradient descent optimization
- Implemented a custom evaluation metric
- Analyzed sensitivity to learning rate and number of iterations.
- Compared results with a scikit-learn Logistic Regression baseline.

### 4. Unsupervised Learning (From Scratch)
- Implemented **K-Means clustering from scratch**.
- Selected number of clusters by plotting elbow graph.
- Analyzed cluster alignment with the target variable (`y`) post-hoc.

---

## Short Summary
This project demonstrates a full machine learning workflow on a real-world dataset, covering data preprocessing, supervised classification, and unsupervised clustering. Logistic Regression was implemented from scratch to predict term deposit subscriptions, while K-Means clustering was used to uncover meaningful customer segments. The results show partial alignment between clusters and subscription outcomes, highlighting the usefulness of unsupervised insights for improving supervised modeling and business decision-making.
