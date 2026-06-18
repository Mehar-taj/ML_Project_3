# 🚗 Car Price Prediction using Machine Learning

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:36D1DC,100:5B86E5&height=250&section=header&text=Car%20Price%20Prediction&fontSize=35&fontColor=ffffff&animation=fadeIn&fontAlignY=40" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.13-blue?logo=python" />
  <img src="https://img.shields.io/badge/Machine%20Learning-Linear%20Regression-orange" />
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-blue?logo=pandas" />
  <img src="https://img.shields.io/badge/NumPy-Numerical%20Computing-blue?logo=numpy" />
  <img src="https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange?logo=scikitlearn" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter" />
  <img src="https://img.shields.io/badge/Status-Completed-success" />
</p>

---

# 📖 Project Overview

This project develops a **Car Price Prediction System using Machine Learning** to estimate the selling price of used cars based on different vehicle specifications.

The model learns patterns from historical car data and predicts the resale value by analyzing important features such as:

- Manufacturing Year
- Present Price
- Kilometers Driven
- Fuel Type
- Seller Type
- Transmission Type
- Number of Previous Owners

A **Linear Regression algorithm** is used to build the prediction model because it is effective for solving regression problems where the output value is continuous.

This project represents my practical learning journey in:

- Artificial Intelligence
- Machine Learning
- Data Science
- Generative AI

The project covers the complete Machine Learning workflow including data collection, data preprocessing, exploratory data analysis, model training, evaluation, and prediction.

---

# 🎯 Project Objectives

The main objectives of this project are:

* Analyze a real-world automobile dataset.
* Perform data exploration and preprocessing.
* Convert categorical features into numerical format.
* Build a regression-based Machine Learning model.
* Predict used car selling prices.
* Evaluate model performance using regression metrics.
* Understand Machine Learning applications in the automobile industry.

---

# 📂 Dataset Information

**Dataset Name:** Car Data Dataset

The dataset contains information about used cars along with their market selling prices.

### Dataset Features

| Feature | Description |
|---------|-------------|
| Car_Name | Name of the vehicle |
| Year | Manufacturing year |
| Present_Price | Current showroom price |
| Kms_Driven | Distance travelled by car |
| Fuel_Type | Type of fuel used |
| Seller_Type | Dealer or Individual seller |
| Transmission | Manual or Automatic |
| Owner | Number of previous owners |
| Selling_Price | Car resale price (Target Variable) |

---

# ⚙️ Technologies Used

<p>

- 🐍 Python
- 📊 NumPy
- 🐼 Pandas
- 🤖 Scikit-Learn
- 📈 Linear Regression
- 📒 Jupyter Notebook

</p>

---

# 🔄 Machine Learning Workflow

## 1. Data Collection

The used car dataset was loaded for analysis and model development.

Libraries used:

```python
import numpy as np
import pandas as pd
from sklearn.linear_model import LinearRegression
from sklearn.model_selection import train_test_split
from sklearn import metrics
````

---

# 2. Exploratory Data Analysis (EDA)

Performed data analysis to understand:

* Dataset structure
* Number of records
* Data types
* Missing values
* Unique categories
* Feature information

Example:

```python
df.info()

df.isnull().sum()
```

---

# 3. Data Preprocessing

Machine Learning algorithms require numerical input, therefore categorical variables were converted into numerical values.

## Encoding Categorical Features

### Seller Type

```
Dealer → 0
Individual → 1
```

### Fuel Type

```
Petrol → 0
Diesel → 1
CNG → 2
```

### Transmission

```
Manual → 0
Automatic → 1
```

---

# 4. Feature Selection

The dataset was divided into:

## Independent Features (Input)

```
Year
Present_Price
Kms_Driven
Fuel_Type
Seller_Type
Transmission
Owner
```

## Dependent Feature (Target)

```
Selling_Price
```

Code:

```python
X = df.drop(['Car_Name','Selling_Price'],axis=1)

Y = df['Selling_Price']
```

---

# 5. Train-Test Split

The dataset was divided into training and testing data.

| Dataset       | Percentage |
| ------------- | ---------- |
| Training Data | 80%        |
| Testing Data  | 20%        |

Code:

```python
X_train, X_test, Y_train, Y_test = train_test_split(
    X,
    Y,
    test_size=0.2,
    random_state=2
)
```

---

# 🤖 Machine Learning Model

## Linear Regression

Linear Regression is a supervised machine learning algorithm used to predict continuous numerical values.

In this project, it learns the relationship between car features and selling price to estimate the resale value of vehicles.

### Advantages:

✔ Simple and efficient
✔ Easy to understand
✔ Works well for regression problems
✔ Provides continuous predictions

---

# 🚀 Model Training

The Linear Regression model was trained using the training dataset.

```python
model = LinearRegression()

model.fit(X_train,Y_train)
```

---

# 📊 Model Evaluation

The model performance was evaluated using:

### R² Score

R² Score measures how well the model explains the variation in the target variable.

Code:

```python
training_prediction = model.predict(X_train)

metrics.r2_score(
    training_prediction,
    Y_train
)
```

Testing:

```python
test_prediction = model.predict(X_test)

metrics.r2_score(
    test_prediction,
    Y_test
)
```

---

# 🚗 Car Price Prediction

The trained model predicts the selling price of a new vehicle based on user input.

Example:

### Input

```python
(2014,3.35,27000,0,0,0,0)
```

### Output

```python
Predicted Car Price: ₹X Lakhs
```

---

# 📈 Results

The model successfully predicts used car prices based on vehicle specifications.

The Linear Regression model demonstrates that Machine Learning can be effectively used for automobile price estimation.

---

# 📁 Project Structure

```
Car-Price-Prediction/
│
├── Car_Price_Prediction.ipynb
├── cardata.csv
├── README.md
├── requirements.txt
└── .gitignore
```

---

# 🚀 Future Improvements

Future enhancements for this project:

* Apply Feature Scaling techniques.

* Perform advanced Exploratory Data Analysis.

* Compare different Machine Learning algorithms:

  * Random Forest Regression
  * XGBoost Regression
  * Gradient Boosting Regression

* Create interactive dashboards.

* Develop a Streamlit web application.

* Deploy the Machine Learning model online.

---

# 📚 Key Learnings

Through this project, I gained practical experience in:

* Data Collection
* Data Cleaning
* Exploratory Data Analysis
* Data Preprocessing
* Feature Engineering
* Regression Algorithms
* Model Evaluation
* Predictive System Development

---

# 🌱 Learning Journey

This project is part of my continuous learning journey in:

✨ Artificial Intelligence (AI)
✨ Machine Learning (ML)
✨ Data Science
✨ Generative AI

Each project helps me improve my problem-solving skills and understand how intelligent systems are developed using real-world data.

---

# 👩‍💻 Author

## Mehar-taj

**Aspiring Data Scientist | Machine Learning Enthusiast | AI & Generative AI Learner**

🔗 GitHub:
[https://github.com/Mehar-taj](https://github.com/Mehar-taj)

🔗 LinkedIn:
[https://www.linkedin.com/in/mehar-taj-a654102b6](https://www.linkedin.com/in/mehar-taj-a654102b6)

---

⭐ If you found this project useful, consider giving it a star and exploring my other Machine Learning projects.

```

This version matches your **Breast Cancer Prediction README style** and is ready for GitHub portfolio use.
```
