# 📊 Comparing Multiple Machine Learning Models for Regression

## 📌 Project Overview
This project focuses on training, evaluating, and comparing multiple regression models to determine the best-performing algorithm for predicting house prices per unit area. The dataset used contains information such as house age, distance to the nearest MRT station, number of convenience stores nearby, latitude, and longitude.

## 📂 Dataset
The dataset consists of **414 entries** with the following features:
- **Transaction date** (converted to year and month)
- **House age** (years)
- **Distance to nearest MRT station** (meters)
- **Number of convenience stores** (count)
- **Latitude** and **Longitude** (location coordinates)
- **House price of unit area** (target variable)

## 🔧 Data Preprocessing
1. Converted the **Transaction date** into **year** and **month**.
2. Scaled numerical features using **StandardScaler** for better model performance.
3. Split data into **training (80%)** and **testing (20%)** sets.

## 🏆 Models Compared
The following regression models were trained and evaluated:
- **Linear Regression** 🏁 (Baseline model)
- **Decision Tree Regressor** 🌳
- **Random Forest Regressor** 🌲🌲
- **Gradient Boosting Regressor** 🚀

## 📊 Model Evaluation
The models were assessed using:
- **Mean Absolute Error (MAE)**: Measures the average absolute differences between actual and predicted values.
- **R² Score**: Indicates how well the model explains the variance in the target variable.

| Model                  | MAE  | R² Score |
|------------------------|------|---------|
| Linear Regression      | 9.75 | 0.53    |
| Decision Tree Regressor | 11.76 | 0.20    |
| Random Forest Regressor | 9.89 | 0.51    |
| Gradient Boosting Regressor | 10.00 | 0.48    |

### 🔥 **Best Model: Linear Regression**
Despite being the simplest model, **Linear Regression** performed best with the lowest **MAE (9.75)** and highest **R² (0.53)**.
## 📌 Requirements
- Python 3.x
- Pandas
- Scikit-learn
- NumPy
