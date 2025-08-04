# 🏡 House Price Prediction using Linear Regression

This project explores a supervised machine learning approach to predict house prices using linear regression. It uses data from the popular **Ames Housing dataset** and is built entirely in Python using scikit-learn, pandas, and matplotlib/seaborn.

---

## 📌 Goal

To build a simple yet effective model that can **predict house prices** based on a few important features, while learning the key steps in a typical machine learning workflow — from EDA to model evaluation.

---

## 🛠️ Tools & Libraries

- Python 🐍
- Pandas & NumPy for data wrangling
- Matplotlib & Seaborn for visualizations
- scikit-learn for model building

---

## 🔍 Dataset

We used the [Ames Housing Dataset](https://www.kaggle.com/datasets/prevek18/house-prices-dataset) which contains various features about homes in Ames, Iowa — such as area, number of rooms, neighborhood, etc.

- `train.csv` — contains features + target `SalePrice`
- `test.csv` — used for predictions (target not provided)

---

## 🚶 Project Workflow

1. **Load Data**  
   We read both the training and test data files and checked for structure, missing values, and feature types.

2. **Data Cleaning & Preparation**  
   - Dropped irrelevant features (like `Id`)
   - Encoded categorical variables using one-hot encoding
   - Ensured train and test had the same features after encoding

3. **Exploratory Data Analysis (EDA)**  
   - Visualized distributions of sale prices
   - Checked correlations
   - Compared average house prices across neighborhoods

4. **Model Training (Linear Regression)**  
   Trained a Linear Regression model using scikit-learn and fit it on the training set.

5. **Model Evaluation**  
   - MAE: \$13,460  
   - RMSE: \$20,956  
   - R² Score: **0.9304**

   The model explains **93% of the variance** in house prices — pretty solid for a basic model!

6. **Test Set Prediction**  
   We used the trained model to predict house prices on the test data and visualized the distribution of predictions.

---

## 📊 Sample Visualizations

- Distribution of house prices  
- Average price by neighborhood  
- Correlation heatmap  
- Comparison of training target vs. test predictions

These help us understand the data and the model's behavior beyond just metrics.

---

## 🧠 Key Takeaways

- Linear regression can perform surprisingly well with well-chosen features
- Data preprocessing (cleaning + encoding) is just as important as model building
- Visualizing both EDA and results makes the work more transparent and easier to communicate

---

## 📁 Folder Structure

