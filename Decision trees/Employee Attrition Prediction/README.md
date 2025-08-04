🧑‍💼 IBM HR Analytics: Employee Attrition Prediction (Decision Tree)
====================================================================
Welcome to this HR analytics project where we dive deep into the IBM Employee Attrition dataset to
build a machine learning model that predicts whether an employee is likely to leave the company. 
This can be incredibly useful for HR departments looking to understand and reduce attrition!

--------------------------------------------------------------------------------------------------------------------

📌 Objective
=============
The primary goal is to use employee records (such as job role, income, satisfaction level, years at company, etc.)
to predict Attrition — whether an employee is likely to stay (0) or leave (1). We’ve used a Decision Tree Classifier
for this task.

---------------------------------------------------------------------------------------------------------------------

## Dataset Used:

Here is the dataset link:
[IBM HR Analytics Employee Attrition & Performance](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

🔍 What This Project Covers
============================
📦 Loading and understanding the IBM dataset
🎨 Beautiful and interactive EDA (Exploratory Data Analysis) to uncover hidden trends
🧹 Proper data preprocessing, including encoding categorical variables
🌳 Training a Decision Tree classifier on training data
📈 Model evaluation using accuracy, precision, recall, and F1-score
📊 Visualizations: Confusion matrix, classification report, feature importances
💾 Saving the trained model for future use

-----------------------------------------------------------------------------------------------------------------------

🧠 Model Performance
=====================
After training and evaluating our model on the test set, here's how it performed:
✅ Accuracy Score: 84.35%

The model does a great job identifying employees who will stay. However, it struggles
with predicting attrition cases, which are relatively few — a classic class imbalance issue.

-------------------------------------------------------------------------------------------------------------------------

📊 Feature Importance
=====================
We’ve also visualized which features were most influential in the model’s decision-making. Features like OverTime, 
JobSatisfaction, YearsAtCompany, and MonthlyIncome play a significant role in determining attrition.

--------------------------------------------------------------------------------------------------------------------------

💾 Model Export
===============
The trained model is saved as:

--"decision_tree_hr_attrition_model.pkl"

This allows us to load it later for predictions without needing to retrain.

---------------------------------------------------------------------------------------------------------------------------

💬 Final Thoughts
=================
This project is a solid example of how machine learning can assist in real-world HR decisions. While our model has decent
accuracy overall, improving attrition detection (class 1) would benefit from more data or advanced techniques like SMOTE,
ensemble models, or cost-sensitive learning.

---------------------------------------------------------------------------------------------------------------------------

Note
=====
There are one visual that is not shown in the notebook because it can't be shown here but wwas shown while wworking on it
in google colab.So,try this in colab,and it will work perfectly fine.

Feel free to explore, improve, or deploy this model!
