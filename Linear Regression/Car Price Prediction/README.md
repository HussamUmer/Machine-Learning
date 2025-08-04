# 🚗 Car Price Prediction using Linear Regression

Welcome! 👋  
This project is a simple, clean implementation of predicting car prices using linear regression — one of the foundational models in machine learning.

---

## 📊 What This Project Does

The goal here was to predict the price of a car based on features like its brand, engine size, fuel type, horsepower, and a bunch of other specs.

We walked through:
- Loading and understanding the dataset
- Cleaning + encoding the data
- Exploring relationships through visuals
- Training a linear regression model
- Evaluating how well the model performs
- Saving the final trained model

---

## 🧪 Dataset Used

A dataset containing various car features like:
- Brand and model
- Fuel type, engine size, horsepower
- Car body, dimensions, drive wheels
- ...and finally, **price** (our target)

---

## 📈 Model Performance

After training and testing, here’s how the model did:

- **Mean Absolute Error (MAE)**: `3988.29`
- **Mean Squared Error (MSE)**: `43,000,397.88`
- **Root Mean Squared Error (RMSE)**: `6,557.47`
- **R² Score**: `0.4553`

✅ This means that on average, the model is off by about **$3,988** and explains nearly **46%** of the variation in car prices — not perfect, but a strong starting point for a simple linear model.

---

## 📊 Visualizations

We used Seaborn and Matplotlib to visualize:
- Price distribution
- Price vs Engine Size
- Fuel type comparisons
- Correlation heatmap
- Brand distribution

All visuals are available inside the notebook and saved in the `/output/visualizations/` folder.

---



## 📂 Project Structure

