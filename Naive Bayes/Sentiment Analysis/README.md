# 📝 Sentiment Classification with Naive Bayes (Amazon & Best Buy Electronics Reviews)


## 📌 Overview

This project aims to detect sentiment (positive or negative) from product reviews collected from Amazon
and Best Buy using Naive Bayes, a popular algorithm in Natural Language Processing (NLP).
- We built a text classification pipeline that:
- Cleans and pre-processes raw review text
- Converts it into numerical features using TF-IDF
- Trains a Multinomial Naive Bayes model
- Evaluates the model on unseen data with strong performance visuals

----------------------------------------------------------------------------------------------------------

## 📦 Dataset Details

- 📁 Source: Public Review Dataset of Amazon & Best Buy electronics
- 🗂️ Size: ~7,300 reviews

🧾 Columns Used:
-----------------
- reviews.text: The written product review
- reviews.rating: A numeric rating (1 to 5)

--------------------------------------------------------------------------------------------------------------

## 🧪 Problem Statement

We framed this as a binary classification problem:

- Ratings ≥ 4 → Positive sentiment (1)
- Ratings < 4 → Negative sentiment (0)
This transformation helps train the model to focus on overall satisfaction rather than specific ratings.

---------------------------------------------------------------------------------------------------------------

## 🔁 Project Workflow

- Data Loading & Cleaning
        Removed missing entries
        Renamed columns for clarity
                   ----------------------------------
- Sentiment Labeling
         Converted numeric ratings to binary sentiment labels (positive/negative)
                    ---------------------------------
- Text Preprocessing
          Lowercased the text
          Removed URLs, numbers, punctuation, and extra whitespace
                     ---------------------------------
- EDA (Exploratory Data Analysis)
          Plotted sentiment distribution (revealed strong class imbalance)
          Visualized review length distribution
                      ---------------------------------
- Train/Test Split
           Used an 80/20 split with stratification to maintain label ratios
                       ---------------------------------
- Feature Engineering
           Used TF-IDF vectorization to convert text into feature vectors
                        ---------------------------------
- Model Training
           Trained a Multinomial Naive Bayes classifier on the TF-IDF vectors
                          --------------------------------
- Evaluation & Visualization
           Accuracy Score: 86.96%
           F1-Score (Positive class): 0.92
                           --------------------------------
- Confusion matrix visualization

---------------------------------------------------------------------------------------------------------

## 📊 Performance Metrics

### ✅ Accuracy Score: 0.8696
--------------------------

### 📄 Classification Report:

              precision    recall  f1-score   support

    Negative       0.52      0.73      0.61       196
    Positive       0.95      0.89      0.92      1230

    accuracy                           0.87      1426
   macro avg       0.74      0.81      0.76      1426
weighted avg       0.89      0.87      0.88      1426

----------------------------------------------------------------------------------------------------------

## 📉 Confusion Matrix:

- The model performs exceptionally well on the positive class.
- Negative class is less represented, resulting in relatively lower precision.

----------------------------------------------------------------------------------------------------------

## ⚠️ Challenges & Fixes

We encountered a few hurdles during this project:

- Labeling Confusion
-----------------------
Initially, there was an attempt to rename the dataset's columns with df.columns = ['review', 'sentiment'], 
which failed because the dataset had more than two columns.
✅ Fixed by selecting only the required columns explicitly.

- Missing Columns in Plotting
--------------------------------
Tried plotting a countplot on a column that didn’t exist (review), which threw a KeyError.
✅ Fixed by double-checking column names and ensuring the correct label column was passed.

- Severe Class Imbalance
---------------------------
Majority of reviews were positive, which led to poor performance on the minority (negative) class.
✅ Acknowledged but not yet resolved. Future improvement could include oversampling or SMOTE to balance classes.

- Text Processing Errors
----------------------------
Some entries were missing or malformed (e.g., non-string values).
✅ Solved by type casting and defensive coding during cleaning.

-----------------------------------------------------------------------------------------------------------------

## 📈 Future Improvements

✅ Balance dataset using SMOTE or class-weighted loss
🧠 Try more advanced models like Logistic Regression, SVM, or XGBoost
📦 Save the trained model using joblib for deployment
📊 Build a Streamlit or Flask app for live sentiment predictions

-----------------------------------------------------------------------------------------------------------------

## 🧠 Final Thoughts

This project was a great demonstration of how simple models like Naive Bayes can still perform surprisingly well on real-world text data — especially when paired with clean preprocessing and solid feature extraction techniques like TF-IDF.


