# 🏥 Medical Insurance Cost Prediction

This project predicts a person's annual medical insurance charges based on factors like their age,
BMI, smoking habits, and more.

---------------------------------------------------------------------------------------------------

## 🧠 What’s the Idea?

Healthcare costs are rising every day, and insurance companies need smarter tools to estimate future expenses.
This project builds a simple yet solid linear regression model to predict these insurance costs,
giving us a glimpse into how data and ML are reshaping real-world decision-making.

----------------------------------------------------------------------------------------------------
## 📦 Dataset Info

The dataset contains real-world insurance data and includes:

- Age
- Gender
- BMI (Body Mass Index)
- Number of children
- Smoking status
- Region of residence
- Medical charges (target)

------------------------------------------------------------------------------------------------------
## 🔍 Step-by-Step Approach

1. Exploratory Data Analysis (EDA)

Before modeling, I explored:

- Average costs across different regions and genders
- How smoking impacts medical charges
- Correlation between numerical features and charges
- Distribution of charges (spoiler: it's skewed!)
  
2. Data Preprocessing

- Converted categorical variables using One-Hot Encoding  
- Standardized the data where needed  
- Split the dataset into 80% training and 20% test

3. Modeling

Used "Linear Regression" for this initial approach. It's simple, interpretable, and fast.

---------------------------------------------------------------------------------------------------
4. Evaluation

Here’s how the model performed:

- "MAE:" 4181.19
- "MSE:" 33,596,915.85
- "RMSE:" 5796.28
- "R² Score:" 0.7836

Not too bad for a linear model.

-----------------------------------------------------------------------------------------------------
## 📈 Visuals Matter

I’ve added several clean and colorful plots:

- Age vs Charges
- BMI vs Charges (highlighting smokers)
- Distribution of Charges
- Actual vs Predicted Charges

These help make sense of the patterns and model behavior.

------------------------------------------------------------------------------------------------------

## 🧪 Future Work

- Try regularized models (Lasso, Ridge)
- Use XGBoost or Random Forests for performance boost
- Add interactivity with Streamlit or Gradio

------------------------------------------------------------------------------------------------------

If you found this project helpful, feel free to ⭐ the repo or suggest improvements!




