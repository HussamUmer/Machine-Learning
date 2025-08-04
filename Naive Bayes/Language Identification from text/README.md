# 🌍 Language Detection using Naive Bayes

Welcome to this fun and insightful machine learning project, where we teach a computer to detect the language
of a given text snippet! This model can identify 17 different languages using simple text samples — from English
to Malayalam to Turkish.

-----------------------------------------------------------------------------------------------------------------------

## 🚀 Project Overview

In this project, we built a multiclass text classification system that predicts the language of a sentence. It’s powered
by the Naive Bayes algorithm and uses TF-IDF vectorization to understand the significance of words.

We used a dataset titled "Language Detection", which includes thousands of labeled sentences across 17 world languages.

-------------------------------------------------------------------------------------------------------------------------

## Dataset Used

This is the link to dataset:
[Language Detection](https://www.kaggle.com/datasets/basilb2s/language-detection)

-------------------------------------------------------------------------------------------------------------------------

## 🧠 Tech Stack Used

- 🐍 Python
- 📊 Pandas, NumPy – for data wrangling
- 📈 Matplotlib, Seaborn – for visualizations
- 🧹 re (regex) – for cleaning text
- 🧠 Scikit-learn – for vectorization and modeling
- 💾 Joblib – to save the model

--------------------------------------------------------------------------------------------------------------------------

## 📊 Exploratory Data Analysis (EDA)

To better understand the dataset, we explored:

✅ Distribution of languages (bar chart)
✍️ Sample sentences from each language

These insights helped ensure balanced representation and gave us a feel for multilingual variance.

---------------------------------------------------------------------------------------------------------------------------

## ⚙️ Preprocessing Steps

- Text cleaning:

        Lowercased all words
        Removed punctuation, digits, links, and extra spaces
            
- Label encoding:

        Converted each language label into a numerical form
        TF-IDF Vectorization:
        Transformed raw sentences into numerical vectors based on term importance across the dataset
        
- Train-Test Split:

         Used an 80/20 split to train and validate the model fairly

----------------------------------------------------------------------------------------------------------------

## 🧪 Model Training

We used the Multinomial Naive Bayes classifier, which is fast, interpretable, and works especially well for text
classification tasks like this one.

-----------------------------------------------------------------------------------------------------------------

## 📈 Model Performance

### ✅ Accuracy: 94.63%
---------------------
The model performed remarkably well, even across less-represented languages.

Overall, languages with fewer samples (like Hindi, Tamil, Turkish) still performed well, showing the robustness
of our pipeline.

-----------------------------------------------------------------------------------------------------------------

## 📦 Saving the Model

To make reuse easy, we saved both the trained model and the TF-IDF vectorizer using joblib. These can be loaded
later to make predictions on new text samples without retraining.

------------------------------------------------------------------------------------------------------------------

## 🤔 Challenges Faced

- ⚠️ Class imbalance: Some languages had far fewer samples than others. We tackled this using stratified splitting
and TF-IDF to reduce sensitivity to size.
- 🔡 Mixed scripts: Languages using non-Latin characters (e.g., Arabic, Hindi) required careful cleaning to retain
meaningful structure.
- 💬 Very short sentences: These were hard to classify, especially if the vocabulary was sparse or ambiguous.

---------------------------------------------------------------------------------------------------------------------

## 💡 What We Learned

- Naive Bayes + TF-IDF = a surprisingly strong baseline for language detection
- Even with limited samples, proper preprocessing and vectorization can achieve excellent accuracy
- Language detection is a practical application of NLP, with real-world use cases in chatbots, browsers, and 
translation tools

-----------------------------------------------------------------------------------------------------------------------


