# 🚗 Car Price Prediction Using Machine Learning

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:2193B0,100:6DD5ED&height=250&section=header&text=Car%20Price%20Prediction%20using%20Machine%20Learning&fontSize=35&fontColor=ffffff&animation=fadeIn&fontAlignY=40" />
</p>

![Python](https://img.shields.io/badge/Python-3.13-blue?style=for-the-badge\&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge\&logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?style=for-the-badge\&logo=numpy)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-F7931E?style=for-the-badge\&logo=scikitlearn)
![Linear Regression](https://img.shields.io/badge/Model-Linear%20Regression-success?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

---

## 📖 Project Overview

This project develops a **Machine Learning-based Car Price Prediction System** that estimates the selling price of used cars using various vehicle characteristics such as manufacturing year, present price, kilometers driven, fuel type, seller type, transmission type, and ownership history.

The model is built using **Linear Regression**, a supervised machine learning algorithm commonly used for regression tasks. This project demonstrates how machine learning can be applied to solve real-world business problems in the automobile industry.

---

## 🎯 Project Objectives

* Analyze historical car sales data.
* Perform data preprocessing and feature encoding.
* Train a Linear Regression model.
* Evaluate model performance using R² Score.
* Build a predictive system for estimating used car prices.

---

## 📂 Dataset Information

The dataset contains details of used cars along with their selling prices.

### Features

| Feature       | Description               |
| ------------- | ------------------------- |
| Car_Name      | Name of the Car           |
| Year          | Manufacturing Year        |
| Present_Price | Current Ex-Showroom Price |
| Kms_Driven    | Distance Driven (in KM)   |
| Fuel_Type     | Petrol / Diesel / CNG     |
| Seller_Type   | Dealer / Individual       |
| Transmission  | Manual / Automatic        |
| Owner         | Number of Previous Owners |
| Selling_Price | Target Variable           |

---

## 🔍 Exploratory Data Analysis (EDA)

The following analysis was performed:

* Dataset overview
* Data type inspection
* Missing value analysis
* Unique category analysis
* Feature understanding

### Basic Analysis

* Seller Type Distribution
* Fuel Type Distribution
* Transmission Type Distribution

---

## 🛠 Data Preprocessing

Several preprocessing steps were performed before training the model:

### Feature Encoding

Categorical variables were converted into numerical values:

| Category   | Encoded Value |
| ---------- | ------------- |
| Dealer     | 0             |
| Individual | 1             |
| Petrol     | 0             |
| Diesel     | 1             |
| CNG        | 2             |
| Manual     | 0             |
| Automatic  | 1             |

---

## 🎯 Feature Selection

Input features (**X**) include:

* Year
* Present Price
* Kms Driven
* Fuel Type
* Seller Type
* Transmission
* Owner

Target variable (**Y**):

* Selling Price

---

## ✂️ Train-Test Split

The dataset was divided into:

* **80% Training Data**
* **20% Testing Data**

This allows the model to learn from historical data and evaluate its performance on unseen data.

```python
X_train, X_test, Y_train, Y_test = train_test_split(
    X, Y,
    test_size=0.2,
    random_state=2
)
```

---

## 🤖 Model Training

A Linear Regression model was trained using the training dataset.

```python
from sklearn.linear_model import LinearRegression

model = LinearRegression()
model.fit(X_train, Y_train)
```

### Algorithm Used

* Linear Regression

---

## 📊 Model Evaluation

The model performance was evaluated using the **R² Score**.

### Training Performance

```python
training_data_prediction = model.predict(X_train)

training_data_accuracy = metrics.r2_score(
    Y_train,
    training_data_prediction
)
```

### Testing Performance

```python
test_data_prediction = model.predict(X_test)

test_data_accuracy = metrics.r2_score(
    Y_test,
    test_data_prediction
)
```

---

## 🚗 Prediction System

The trained model can predict the selling price of a used car based on user-provided specifications.

### Sample Input

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

### Prediction Process

```python
input_data_array = np.asarray(input_data)

input_data_reshape = input_data_array.reshape(1, -1)

prediction = model.predict(input_data_reshape)

print(prediction)
```

### Sample Output

```text
Predicted Selling Price: ₹2.75 Lakhs
```

---

## 📈 Results

The model successfully predicts used car prices using vehicle specifications and historical market data.

### Performance Metrics

| Metric            | Result              |
| ----------------- | ------------------- |
| Training R² Score | High Accuracy       |
| Testing R² Score  | Good Generalization |

---

## 📚 Key Learnings

Through this project, I gained practical experience in:

* Data Cleaning
* Data Preprocessing
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Feature Encoding
* Regression Analysis
* Linear Regression
* Model Evaluation
* Predictive Analytics

---

## 🚀 Future Improvements

Possible enhancements include:

* Feature Scaling
* Feature Engineering (Car Age)
* Random Forest Regression
* XGBoost Regression
* Hyperparameter Tuning
* Streamlit Web Application
* Model Deployment on Cloud

---

## 📁 Project Structure

```text
Car-Price-Prediction/
│
├── Car_Price_Prediction.ipynb
├── cardata.csv
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 🛠 Technologies Used

* Python
* NumPy
* Pandas
* Scikit-Learn
* Linear Regression
* Jupyter Notebook
* Git & GitHub

---

## ✅ Conclusion

Successfully developed a **Car Price Prediction System** using Machine Learning. The model estimates the selling price of used cars based on vehicle characteristics and demonstrates the practical application of regression techniques in solving real-world automobile industry problems.

---

## 👩‍💻 Author

### Mehar-taj

Aspiring Data Scientist | Machine Learning Enthusiast | AI & Generative AI Learner

GitHub: https://github.com/Mehar-taj

LinkedIn: https://www.linkedin.com/in/mehar-taj-a654102b6

---

⭐ If you found this project useful, consider giving it a star and exploring my other AI and Machine Learning projects.


⭐ If you found this project helpful, consider giving it a Star!
