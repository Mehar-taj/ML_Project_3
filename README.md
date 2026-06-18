# 🚗 Car Price Prediction using Machine Learning

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:36D1DC,100:5B86E5&height=250&section=header&text=Car%20Price%20Prediction&fontSize=35&fontColor=ffffff&animation=fadeIn&fontAlignY=40" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.13-blue?logo=python" />
  <img src="https://img.shields.io/badge/Machine%20Learning-Linear%20Regression-orange" />
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-blue?logo=pandas" />
  <img src="https://img.shields.io/badge/NumPy-Numerical%20Computing-blue?logo=numpy" />
  <img src="https://img.shields.io/badge/Scikit--Learn-ML-orange?logo=scikitlearn" />
  <img src="https://img.shields.io/badge/Status-Completed-success" />
</p>

---

## 📖 Project Overview

This project develops a **Car Price Prediction System** using Machine Learning techniques to predict the selling price of used cars based on various vehicle features.

The model analyzes important factors such as **manufacturing year, present price, kilometers driven, fuel type, seller type, transmission type, and ownership history** to estimate the resale value of a vehicle.

A **Linear Regression algorithm** is implemented to build the prediction model and understand the relationship between car specifications and market prices.

As part of my continuous learning journey in **Artificial Intelligence, Machine Learning, Data Science, and Generative AI**, this project demonstrates a complete machine learning workflow including data preprocessing, feature engineering, model training, evaluation, and prediction.

---

# 🎯 Project Objectives

* Analyze a real-world automobile dataset.
* Perform data cleaning and preprocessing.
* Convert categorical data into numerical format.
* Build a regression model using Linear Regression.
* Evaluate model performance using regression metrics.
* Develop a system to predict used car prices.
* Understand practical applications of Machine Learning in the automobile industry.

---

# 📂 Dataset Information

**Dataset:** Car Data Dataset

The dataset contains information about used cars along with their selling prices.

### Features:

| Feature | Description |
|---------|-------------|
| Car_Name | Name of the car |
| Year | Manufacturing year |
| Present_Price | Current car price |
| Kms_Driven | Total kilometers driven |
| Fuel_Type | Fuel category |
| Seller_Type | Dealer or Individual |
| Transmission | Manual or Automatic |
| Owner | Previous ownership count |
| Selling_Price | Target variable |

---

# ⚙️ Technologies Used

* Python
* NumPy
* Pandas
* Scikit-Learn
* Linear Regression
* Jupyter Notebook

---

# 🔄 Project Workflow

## 1. Data Collection

* Loaded the used car dataset.
* Imported required Python libraries for analysis and modeling.

---

## 2. Data Exploration (EDA)

Performed exploratory data analysis to understand:

* Dataset structure.
* Data types.
* Missing values.
* Unique categories.
* Feature relationships.

---

## 3. Data Preprocessing

Categorical features were converted into numerical values.

### Encoding:

**Seller Type**


Dealer → 0
Individual → 1


**Fuel Type**


Petrol → 0
Diesel → 1
CNG → 2


**Transmission**


Manual → 0
Automatic → 1


---

## 4. Feature Selection

Separated independent features and target variable.

### Input Features:

* Year
* Present Price
* Kms Driven
* Fuel Type
* Seller Type
* Transmission
* Owner


### Target Variable:

* Selling Price

---

## 5. Train-Test Split

The dataset was divided into:

| Dataset | Percentage |
|---------|------------|
| Training Data | 80% |
| Testing Data | 20% |

Training data is used for learning, while testing data evaluates model performance.

---

## 6. Model Training

A **Linear Regression Model** was trained using the training dataset.

Linear Regression is a supervised learning algorithm used for predicting continuous numerical values by finding relationships between input features and output variables.

---

## 🤖 Machine Learning Model

## Linear Regression

Linear Regression predicts the selling price of a car by learning patterns between vehicle features and historical prices.

### Advantages:

* Simple and efficient algorithm.
* Easy interpretation.
* Works well for regression problems.
* Provides continuous price predictions.

---

# 📊 Model Evaluation

The model performance was evaluated using:

* R² Score

### Performance:

| Metric | Result |
|--------|--------|
| Training Accuracy | Calculated using R² Score |
| Testing Accuracy | Calculated using R² Score |

The model demonstrates the ability to predict used car prices based on vehicle specifications.

---

# 🚗 Sample Prediction

### Input:

Vehicle details:

```python
(2014, 3.35, 27000, 0, 0, 0, 0)
Output:
Predicted Car Price: ₹X Lakhs
📁 Project Structure
Car-Price-Prediction/
│
├── Car_Price_Prediction.ipynb
├── cardata.csv
├── README.md
├── requirements.txt
└── .gitignore
🚀 Future Improvements
Apply Feature Scaling techniques.
Compare multiple regression algorithms:
Random Forest Regression
XGBoost Regression
Gradient Boosting
Add data visualization.
Create an interactive Streamlit web application.
Deploy the model using cloud platforms.
📚 Key Learnings

Through this project, I gained practical experience in:

Data Cleaning
Exploratory Data Analysis
Data Preprocessing
Feature Engineering
Regression Algorithms
Model Evaluation
Predictive System Development
🌱 Learning Journey

This project is part of my ongoing journey in:

Artificial Intelligence (AI)
Machine Learning (ML)
Data Science
Generative AI

Each project helps me improve my understanding of solving real-world problems using intelligent data-driven solutions.

👩‍💻 Author
Mehar-taj

Aspiring Data Scientist | Machine Learning Enthusiast | AI & Generative AI Learner

GitHub: https://github.com/Mehar-taj

LinkedIn: https://www.linkedin.com/in/mehar-taj-a654102b6

⭐ If you found this project useful, consider giving it a star and exploring my other Machine Learning projects.


This will give your GitHub repository the same **professional portfolio style** as your Breast Cancer Pre
