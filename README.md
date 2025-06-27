# 🏡 California Housing Price Prediction using SVM

This project uses **Support Vector Regression (SVR)** from `scikit-learn` to predict house prices based on features from the **California Housing Dataset**. The goal is to build a regression model that can estimate median house values across various districts in California.

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Numpy-013243?style=flat-square&logo=numpy&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Matplotlib-007ACC?style=flat-square&logo=matplotlib&logoColor=white"/>
  <img src="https://img.shields.io/badge/Seaborn-76B900?style=flat-square"/>
</p>

---

## 🧠 What is Support Vector Regression?

**Support Vector Regression (SVR)** is a type of Support Vector Machine used for predicting continuous values. It tries to fit the best line or curve within a threshold (margin of tolerance) so that the majority of data points fall inside that margin.

---

## 🏘️ About the Dataset

We use the **California Housing Dataset** from `sklearn.datasets.fetch_california_housing`. It contains real estate data collected from California districts.

### 📌 Features:

| Column Name             | Description                                     |
|-------------------------|-------------------------------------------------|
| `MedInc`                | Median income in block                         |
| `HouseAge`              | Median house age in block                      |
| `AveRooms`              | Average number of rooms per household          |
| `AveBedrms`             | Average number of bedrooms per household       |
| `Population`            | Block population                               |
| `AveOccup`             | Average number of household members            |
| `Latitude`              | Block latitude                                 |
| `Longitude`             | Block longitude                                |

🎯 **Target Column**: `MedHouseVal` – Median house value (in $100,000s)

---

## 🚀 Project Workflow

1. Load the California Housing dataset using `fetch_california_housing()`
2. Split data into training and test sets
3. Train an SVR model using a kernel (like `'linear'` or `'rbf'`)
4. Predict on test data
5. Evaluate model performance using R² Score and MSE
6. Visualize predictions vs actual values
