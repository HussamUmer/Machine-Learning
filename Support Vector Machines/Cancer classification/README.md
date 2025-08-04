# 🧬 Breast Cancer Classification using Support Vector Machine (SVM)

This project tackles a life-critical problem: predicting whether a tumor is malignant or benign using the Breast
Cancer Wisconsin Dataset. Using a Support Vector Machine (SVM), we built a high-performing classification model 
that helps us make predictions based on medical measurements such as radius, texture, symmetry, and more.

------------------------------------------------------------------------------------------------------------------

## 🔍 Objective

To develop an intelligent classification system using SVM that can accurately detect malignant (cancerous) and benign
(non-cancerous) tumors from a set of medical features.

----------------------------------------------------------------------------------------------------------------------

## 🧠 What’s Inside?

- Clean, commented, and readable code with human-friendly explanations.
- Exploratory Data Analysis (EDA) with visualizations.
- Data scaling with StandardScaler.
- Model training using SVC from scikit-learn.
- Model evaluation with accuracy score, classification report, and confusion matrix.
- Bonus: Decision boundary visualization using PCA.
- Bonus: Model saving and loading using joblib.

-------------------------------------------------------------------------------------------------------------------------

## 📦 Dataset Info

Dataset used: Breast Cancer Wisconsin Diagnostic Dataset

- Total samples: 569
- Features: 30 numerical features (e.g., radius, texture, area, smoothness, etc.)

Target classes:
---------------
- 0: Malignant
- 1: Benign

Dataset link:[Breast Cancer Wisconsin (Diagnostic) Data Set](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)

--------------------------------------------------------------------------------------------------------------------------

## 📊 Exploratory Data Analysis

We explored the dataset to understand the distributions of:

- Diagnosis label counts (Malignant vs. Benign)
- Feature correlations using a heatmap
- Mean values of features for each class using violin plots

These visuals helped us identify patterns and understand how features differ across classes.

--------------------------------------------------------------------------------------------------------------

## ⚙️ Model Pipeline

#### 1. Data Preparation

- Checked for missing values.
- Labeled diagnosis as 0 (Malignant) and 1 (Benign).
- Scaled features using StandardScaler.

#### 2. Model Training

- Used SVC(kernel='linear') to train an SVM classifier.
- Training/testing split: 80/20

#### 3. Evaluation

- ✅ Accuracy Score: 0.9736


- 💯 Overall accuracy: 97.36%
- ✅ Confusion Matrix: Visualized with seaborn to show true positives and false negatives clearly.

-------------------------------------------------------------------------------------------------------------

## 📉 Bonus: Visualizing Decision Boundary

To visualize how the SVM separates the classes, we reduced features to 2 dimensions using PCA and then plotted
the decision boundary. This gives a nice visual understanding of how SVM draws the "line" (or hyperplane) 
between the two tumor classes.

--------------------------------------------------------------------------------------------------------------

## 💾 Model Saving

We saved the trained model and scaler using joblib:

- svm_cancer_model.pkl
- svm_scaler.pkl
This allows for easy reuse of the model without retraining.

------------------------------------------------------------------------------------------------------------------------

## 🛠 Issues Faced

- Initially, visualizing decision boundaries was impossible due to the high-dimensional nature of the data (30 features).
We solved this using PCA to reduce the dimensions to 2D.

- Class imbalance wasn’t a major issue, but we still monitored it using the confusion matrix to ensure fair performance
across both classes.

---------------------------------------------------------------------------------------------------------------------------

## 🚀 Future Improvements

- Deploy the model via a simple Flask web app or Streamlit interface.
- Add ROC and AUC curve evaluation.
- Hyperparameter tuning with GridSearchCV.

---------------------------------------------------------------------------------------------------------------------------
