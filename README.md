# 🏋️ Calorie Burn Prediction - Kaggle Playground Series 2025

This repository contains the solution to the [Kaggle Playground Series - January 2025](https://www.kaggle.com/competitions/playground-series-s5e5/overview) competition. The objective is to predict how many calories a person burns during a workout session based on physiological and biometric features.

## 🧠 Problem Statement

The challenge is to build a regression model that predicts calorie expenditure using features such as:
- Age
- Height
- Weight
- Duration
- Heart Rate
- Body Temperature
- Sex

### 📊 Evaluation Metric

The competition uses **Root Mean Squared Logarithmic Error (RMSLE)** as the evaluation metric:

\[
\text{RMSLE} = \sqrt{\frac{1}{n} \sum_{i=1}^n (\log(\hat{y}_i + 1) - \log(y_i + 1))^2}
\]

---

## 🔍 Exploratory Data Analysis

- Correlation heatmap to understand feature relationships
- Scatter plots of features vs. calories burned
- Data cleaning and dropping non-numeric/categorical columns

---

## ⚙️ Feature Engineering

- One-hot encoding for `Sex`
- Dropped non-informative or redundant columns like `id`
- Normalized/standardized continuous features

---

## 🧪 Model Training

Tested and compared multiple regression models, including:

- XGBoost Regressor (final choice)
- GridSearchCV for parameter tuning
- Evaluation with RMSE and RMSLE

---

## 📈 Results

Achieved a competitive RMSLE score with XGBoost after tuning. Performance plots and metrics are included in the notebook.

---

## 💡 Future Work

- Incorporate domain knowledge for additional feature engineering
- Try ensemble models (e.g., blending XGBoost with LightGBM)
- Feature selection or PCA to reduce dimensionality

