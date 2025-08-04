# 🏦 Loan Approval Prediction using Decision Tree

Welcome to the Loan Prediction Project, where we take raw applicant data and build a model to 
predict whether a loan will be approved or not. If you've ever wondered how banks make these 
decisions, here's your chance to simulate it using machine learning!

---------------------------------------------------------------------------------------------------

## 🎯 Goal of the Project

The goal is to predict loan approval outcomes (Yes or No) based on features like applicant income,
credit history, employment details, and more — using a Decision Tree Classifier.

This model can be a handy tool for automating the decision-making process in financial institutions 
or as a learning milestone for anyone diving into classification problems in ML.

----------------------------------------------------------------------------------------------------

## 📊 What’s Covered

In this project, you’ll find:
📂 Cleaned and preprocessed training data (no test split used)
🎨 Interactive and colorful EDA (Exploratory Data Analysis)
🌲 A well-tuned Decision Tree for classification
📈 Visual insights into feature importance and tree structure
🧠 Full model evaluation on the training dataset

------------------------------------------------------------------------------------------------------

## 🔎 Key Features of the Data

-Categorical variables like Gender, Married, Education, Self_Employed, etc. were properly encoded.
-Numerical variables like ApplicantIncome, LoanAmount, and Credit_History were analyzed and visualized to identify patterns.
-Missing values were filled using smart imputation techniques (mode for categorical, median for numerical).
-Loan_ID was removed since it had no predictive value.

Here is the dataset link:
[Loan Prediction Problem Dataset](https://www.kaggle.com/datasets/altruistdelhite04/loan-prediction-problem-dataset)

--------------------------------------------------------------------------------------------------------

## 📊 Model Evaluation

After training our Decision Tree on the complete training set, here’s how the model performed:
✅ Accuracy Score: 82.25%
🎯 Precision (Class 0 - Not Approved): 90%
🎯 Recall (Class 0): 48%
✅ Precision (Class 1 - Approved): 81%
✅ Recall (Class 1): 98%
🔁 F1-Score (Class 1): 88%

## Interpretation:

The model is especially strong at identifying approved loans, which is crucial for minimizing false
negatives in a real-world setting. While recall for non-approved loans is lower, this gives us a great
foundation to build on with further tuning or ensembling.

----------------------------------------------------------------------------------------------------------

## 📌 Highlights

📍 Visualized the decision tree structure to make the decision-making process interpretable.
🌟 Generated a feature importance chart to show which factors influence loan decisions the most.
🧪 Evaluation focused only on the training set, making this a pure supervised learning task.

----------------------------------------------------------------------------------------------------------
