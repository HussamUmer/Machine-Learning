# 🍷 Red Wine Quality Prediction using Random Forest

## 📌 Project Overview

In this project, we aim to predict the quality of red wine using a Random Forest classification model. The dataset
we're working with, the Red Wine Quality dataset, contains various physicochemical properties of wine such as 
acidity, sugar, alcohol, and pH, along with a quality score given by wine tasters.

Our task is to classify whether a wine is of low (0) or high (1) quality based on its features.

--------------------------------------------------------------------------------------------------------------------

## 📁 Dataset

- Name: Red Wine Quality
- Source: UCI Machine Learning Repository
- Samples: ~1600 red wine entries

Features:

- fixed acidity, volatile acidity, citric acid, residual sugar, chlorides, free sulfur dioxide, total sulfur dioxide,
density, pH, sulphates, alcohol

- Target: quality (converted to binary: good vs. bad)

Dataset Link:[Red Wine Quality](https://www.kaggle.com/datasets/uciml/red-wine-quality-cortez-et-al-2009)

----------------------------------------------------------------------------------------------------------------------

## 🧠 Algorithm Used

Random Forest Classifier: An machine learning method that builds multiple decision trees and merges their outputs to
get a more accurate and stable prediction.

-----------------------------------------------------------------------------------------------------------------------

## 📊 Exploratory Data Analysis (EDA)

We visualized the distribution of all input features to understand:
1. The skewness or spread of features like alcohol, pH, and acidity.
2. Correlations between different features and the wine quality.
3. Imbalance in the quality classes.

EDA helped us identify:

1. Alcohol and sulphates were positively associated with better quality wines.
2. Most quality scores clustered around 5 and 6 .

-------------------------------------------------------------------------------------------------------------------------

## 🧪 Model Evaluation Results

#### ✅ Accuracy Score: 0.9437
#### 📄 Classification Report:


              precision    recall  f1-score   support
              ---------    ------  --------   --------
           0       0.95      0.99      0.97       277
           1       0.93      0.63      0.75        43

    accuracy                           0.94       320
  

#### 🔍 Interpretation:

1. The model performs very well overall, especially in identifying low-quality wines.
2. Precision for high-quality wine is solid (0.93), but recall is lower (0.63), meaning it misses some high-quality wines.
3. Class imbalance (more low-quality than high-quality) likely contributes to this.

--------------------------------------------------------------------------------------------------------------------------

## ⚠️ Challenges and Issues

- 📉 Class Imbalance

1. The dataset contains many more low-quality wines than high-quality ones.
2. This imbalance can cause the model to favor the majority class, reducing recall on minority (good quality) wines.

- ⚙️ Algorithmic Limits

Random Forests are excellent with tabular data, but:

   1. They don’t extrapolate well for unseen patterns.
   2. Feature importance may be biased toward features with more levels or wider ranges.

- 🧪 Potential Improvements

1. Try SMOTE or class weighting to handle imbalance.
2. Tune hyperparameters using GridSearchCV.
3. Test other models like Gradient Boosting or XGBoost.
4. Consider reframing as a regression problem if quality scores are treated as ordinal.

---------------------------------------------------------------------------------------------------------------------------

## 🙌 Final Thoughts

This project demonstrates how Random Forests can be used for real-world classification problems and how EDA, evaluation
metrics, and model tuning are critical for building a reliable pipeline. Although we're getting strong performance, the
class imbalance is a reminder that high accuracy isn't everything—we must also pay close attention to recall and f1-score,
especially when the minority class holds more importance (as it would in quality assurance settings).

---------------------------------------------------------------------------------------------------------------------------
