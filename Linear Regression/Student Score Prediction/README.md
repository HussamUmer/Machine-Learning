# 🎓 Student Performance Prediction

Welcome to this machine learning project where we explore how different factors affect student academic performance — and try to **predict their exam scores** based on that! 📚

---

## 🧠 What’s This About?

We used a dataset that includes student demographic details (like gender, ethnicity, parental education), as well as school-related factors like:
- 🧪 Whether the student completed a test preparation course
- 🍽️ Lunch type (standard or free/reduced)
- 📊 Final scores in **math**, **reading**, and **writing**

The goal: **Predict the average exam score** using linear regression.

---

## Dataset Used:

[Students Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)

---

## 🔍 Key Insights from the Data

- Students who completed the test prep course **scored noticeably higher** 📈
- A standard lunch correlated with better writing and reading performance 🍱
- Parental education level showed **some influence** on scores, especially math 🧠
- Gender differences were visible — but not always consistent across subjects 👩‍🎓👨‍🎓

We used **colorful and clear visualizations** to highlight these relationships!

---

## 🛠️ Model & Results

We trained a simple **Linear Regression** model and tested it on unseen data.

### 📈 Final Evaluation Metrics:
- **Mean Absolute Error (MAE)**: `10.49`
- **Root Mean Squared Error (RMSE)**: `13.40`
- **R² Score**: `0.1622`

This means our predictions are **roughly 10–13 points off** from actual scores — not bad, but there's definitely room to grow with more features or advanced models.

---

## 💼 Technologies Used

- Python 🐍
- pandas, seaborn, matplotlib for data wrangling & visualization
- scikit-learn for model training and evaluation
- Jupyter Notebook / Google Colab

---

## 🤔 What Could Be Better?

- Adding more variables like study time, class participation, etc.
- Trying other models (Random Forest, Gradient Boosting)
- Hyperparameter tuning

---

Thanks for visiting! ✨  
Feel free to fork or clone the project and experiment further.


