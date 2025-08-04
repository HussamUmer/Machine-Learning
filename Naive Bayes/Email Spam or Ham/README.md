# 💌 Email Spam Detection using Naive Bayes

Welcome to the Email Spam Detection project! In this notebook, we take a classic NLP (Natural Language Processing)
problem and use a Naive Bayes classifier to predict whether a given email is spam or not. The goal is to train a 
reliable and efficient model that helps filter out spam messages from our inbox.

-------------------------------------------------------------------------------------------------------------------

## 🧠 What This Project Covers

** A real-world labeled dataset of emails (ham vs spam)
** Text preprocessing using NLP techniques
** Visual exploration of the most common words in spam and non-spam emails
** Feature extraction using TF-IDF
** Training a Multinomial Naive Bayes model
** Evaluating the model with accuracy, precision, recall, and F1-score
** Confusion matrix visualization
** Saving the trained model for future use

----------------------------------------------------------------------------------------------------------------------

## ✅ Dataset Used

Here is the dataset link:
[SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)

## 📊 Model Evaluation Summary

The model performed very well on the unseen test set. Here's a breakdown of the performance:
✅ Accuracy: 95.16% — This means the model correctly classified about 95 out of every 100 emails.

Detailed Breakdown:
-------------------

For ham emails (not spam):
---------------------------
** Precision: 0.95 → Out of all emails predicted as ham, 95% were truly ham.
** Recall: 1.00 → The model correctly identified all the actual ham emails.
** F1-score: 0.97 → Strong harmonic balance between precision and recall.

For spam emails:
----------------
** Precision: 1.00 → Every email predicted as spam was actually spam.
** Recall: 0.64 → The model caught 64% of the actual spam emails.
** F1-score: 0.78 → Still a solid result, though there's room to improve recall.

Macro Average (unweighted mean across classes):
-----------------------------------------------
** Precision: 0.97
** Recall: 0.82
** F1-score: 0.88

Weighted Average (accounts for class imbalance):
------------------------------------------------
** Precision: 0.95
** Recall: 0.95
** F1-score: 0.95

---------------------------------------------------------------------------------------------------------------

## 🧾 Key Takeaways

** The model is highly accurate, with very few false positives or negatives.
** It has a perfect precision score on spam emails, meaning it's very cautious when labeling something as spam.
** There's some room to improve recall for spam detection (catching more spam), possibly by adjusting thresholds 
or using ensemble methods.
** The Naive Bayes model is fast, lightweight, and interpretable — great for text classification.

-----------------------------------------------------------------------------------------------------------------

## 📦 What’s Inside

This project includes:

** Cleaned and preprocessed email dataset
** TF-IDF based feature engineering
** Training using MultinomialNB from scikit-learn
** Evaluation and visualization of the results
** Saved model (spam_classifier_nb.pkl) and vectorizer (tfidf_vectorizer.pkl) for deployment or inference

--------------------------------------------------------------------------------------------------------------------

💡 Next Steps
=============
** Try using n-grams in vectorization for better context
** Experiment with different models like SVM or logistic regression
** Integrate the model into a simple web interface or email client plugin

--------------------------------------------------------------------------------------------------------------------
