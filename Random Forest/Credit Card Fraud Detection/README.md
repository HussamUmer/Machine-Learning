# 💳 Credit Card Fraud Detection using Random Forest

## 🧠 Overview

This project focuses on detecting fraudulent credit card transactions using a Random Forest Classifier. The dataset
contains anonymized features of transactions made by European cardholders over two days. Due to the sensitive nature
of financial data, features such as transaction ID and user information are not included.

Our goal is to build a highly accurate and robust model that can spot fraud cases in real-time, even when such cases
are extremely rare.

-----------------------------------------------------------------------------------------------------------------------

## 📁 Dataset Summary

- Name: Credit Card Fraud Detection
Size: 150MB
Samples: 284,807 transactions
Features: 30 numerical features (V1–V28 are PCA-transformed)

- Label:

0 = Genuine transaction
1 = Fraudulent transaction

- Class Imbalance:

99.8% are genuine
0.2% are fraud

----------------------------------------------------------------------------------------------------------------------

## 🔗 Dataset on Kaggle

[]()

----------------------------------------------------------------------------------------------------------------------

🔍 What’s inside?
==================
This project includes:
📊 Exploratory Data Analysis (EDA) to understand class imbalance and feature distribution
🌲 Random Forest classifier with tuned parameters
✂️ Train/test split using stratification to maintain class balance
📈 Evaluation using accuracy, precision, recall, f1-score, and confusion matrix
🌟 Feature importance visualization
💾 Model saving for future deployment

-------------------------------------------------------------------------------------------------------------------------

📉 Model Performance
=====================
Our trained Random Forest model performs exceptionally well on the test set:

Metric	Score
--------------
✅ Accuracy	0.9996
🎯 Precision (Fraud)	0.94
🔁 Recall (Fraud)	0.82
🧮 F1-Score (Fraud)	0.87

📄 Classification Report:
--------------------------

                 precision    recall  f1-score   support
                 ---------    ------  ---------  --------
           0       1.00        1.00      1.00     56864
           1       0.94        0.82      0.87        98

    accuracy                             1.00     56962
   macro avg       0.97        0.91      0.94     56962
weighted avg       1.00        1.00      1.00     56962
✅ The model achieves very high accuracy, and more importantly, a strong F1-score for the minority (fraud) class,
which is what really matters in this domain.

-------------------------------------------------------------------------------------------------------------------------

📌 Challenges Tackled
=======================
1. Severe class imbalance: Less than 0.2% of the transactions are fraudulent. This required careful evaluation beyond
just accuracy.
2. Anonymized data: Since the features are PCA-transformed, feature interpretability is limited — we focused on pattern
recognition instead of semantics.
3. False positives vs false negatives: In real-world settings, catching fraud (recall) is more important than a small
number of false alarms.

--------------------------------------------------------------------------------------------------------------------------

📊 Visualizations Included
===========================
1. Class distribution plot to visualize imbalance
2. Correlation matrix heatmap
3. Confusion matrix
4. Feature importance plot

These help understand the model’s behavior and dataset characteristics better.

---------------------------------------------------------------------------------------------------------------------------

💾 Model Saving
================
The trained model was saved as random_forest_fraud_model.pkl, so it can be reused later for inference or deployment.

---------------------------------------------------------------------------------------------------------------------------

📌 Final Thoughts
===================
Random Forest proved to be an excellent choice for this problem. Even without complex tuning or oversampling techniques,
it generalizes well and achieves impressive recall on fraud detection — a critical aspect in real-world applications.

In future iterations, one could explore:
----------------------------------------
1. Oversampling techniques like SMOTE
2. Cost-sensitive learning
3. Gradient boosting models (e.g., XGBoost, LightGBM)
4. Real-time streaming detection pipelines

----------------------------------------------------------------------------------------------------------------------------
