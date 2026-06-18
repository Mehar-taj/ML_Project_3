# 🚗 Car Price Prediction Using Machine Learning

![Banner](assets/car-price-prediction-banner.png)

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge\&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-orange?style=for-the-badge\&logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-blue?style=for-the-badge\&logo=numpy)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange?style=for-the-badge\&logo=scikitlearn)
![Linear Regression](https://img.shields.io/badge/Model-Linear%20Regression-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

---

## 📖 Project Overview

This project develops a Machine Learning model to predict the selling price of used cars based on various vehicle characteristics such as manufacturing year, present price, kilometers driven, fuel type, seller type, transmission type, and ownership history.

The model uses **Linear Regression** to estimate car prices accurately and demonstrates the practical application of Machine Learning in the automobile industry.

---

## 🎯 Project Objective

* Analyze historical used-car data.
* Build a regression model for price prediction.
* Evaluate model performance using R² Score.
* Create a predictive system for estimating car selling prices.

---

## 📂 Dataset Information

The dataset contains information about used cars, including:

* Car Name
* Year of Manufacture
* Present Price
* Kilometers Driven
* Fuel Type
* Seller Type
* Transmission Type
* Owner Count
* Selling Price (Target Variable)

---

## 🛠️ Technologies Used

* Python
* NumPy
* Pandas
* Scikit-Learn
* Linear Regression
* Jupyter Notebook

---

## 🔄 Data Preprocessing

The following preprocessing steps were performed:

* Handling missing values
* Encoding categorical features
* Feature selection
* Splitting data into training and testing sets

### Encoded Features

| Feature    | Encoding |
| ---------- | -------- |
| Dealer     | 0        |
| Individual | 1        |
| Petrol     | 0        |
| Diesel     | 1        |
| CNG        | 2        |
| Manual     | 0        |
| Automatic  | 1        |

---

## 🤖 Model Training

The model was trained using:

```python
from sklearn.linear_model import LinearRegression

model = LinearRegression()
model.fit(X_train, Y_train)
```

### Algorithm Used

* Linear Regression

---

## 📊 Model Evaluation

The model performance was evaluated using:

* R² Score

### Results

| Metric            | Score     |
| ----------------- | --------- |
| Training R² Score | Excellent |
| Testing R² Score  | Excellent |

---

## 🚗 Car Price Prediction System

Example Input:

```python
input_data = (
    2014,
    3.35,
    27000,
    0,
    0,
    0,
    0
)
```

Example Output:

```text
Predicted Selling Price: ₹X.XX Lakhs
```

---

## 📁 Project Structure

```text
Car-Price-Prediction/
│
├── Car_Price_Prediction.ipynb
├── cardata.csv
├── README.md
├── requirements.txt
└── assets/
    └── car-price-prediction-banner.png
```

---

## 🚀 Future Improvements

* Feature Engineering
* Random Forest Regressor
* XGBoost Regressor
* Hyperparameter Tuning
* Streamlit Web Application
* Cloud Deployment

---

## 📚 Key Learnings

Through this project, I gained hands-on experience in:

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Feature Encoding
* Regression Modeling
* Model Evaluation
* Predictive Analytics
* Real-World Machine Learning Applications

---

## ✅ Conclusion

Successfully developed a Car Price Prediction System using Machine Learning. The model predicts used-car prices based on vehicle specifications and demonstrates how regression techniques can be applied to solve real-world business problems.

---

### 👩‍💻 About Me

This project is part of my Machine Learning, Data Science, and Generative AI learning journey, where I continuously build real-world projects to strengthen my AI skills and portfolio.

⭐ If you found this project useful, consider giving it a star!
