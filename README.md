# 🏡 Real Estate Price Predictor

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![ML Model](https://img.shields.io/badge/Model-Linear%20Regression-orange.svg)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

A machine learning project designed to predict real estate prices based on various features such as location, square footage, number of bedrooms (BHK), and bathrooms. This project demonstrates a practical application of regression models and data preprocessing techniques.

---

## 📌 Table of Contents

- [Project Introduction](#project-introduction)
- [What This Does](#what-this-does)
- [Source of Data](#source-of-data)
- [Model Testing & Comparisons](#model-testing--comparisons)
- [Example Results](#example-results)
- [Clone This Repository](#Clone-This-Repository)
- [Author](#Author)

---

## 📖 Project Introduction

This notebook-based ML model allows users to estimate house prices for different locations by entering key features. It implements data preprocessing, visualization, and a predictive pipeline using **Linear Regression** and other comparison models.

---

## 🔍 What This Does

- Cleans and preprocesses raw housing data
- Reduces location dimensionality
- Removes price per sqft and bathroom-based outliers
- Implements a linear regression model to predict price
- Compares it with other models (Ridge, Lasso, Decision Tree)
- Saves the trained model using `joblib`

---

## 📊 Source of Data

The dataset includes the following columns:

- `location`: Categorical location names
- `total_sqft`: Total built-up area
- `bath`: Number of bathrooms
- `bhk`: Number of bedrooms
- `price`: Price in Lakhs

Preprocessing steps applied:

- Handling missing values
- Location grouping (`other`)
- Converting sqft ranges to numeric
- Filtering extreme outliers

---

## 📈 Model Testing & Comparisons

The project compares multiple algorithms:

| Algorithm        | R² Score (approx) |
|------------------|------------------|
| Linear Regression| 0.84             |
| Lasso Regression | 0.82             |
| Ridge Regression | 0.83             |
| Decision Tree    | 0.75             |

> Linear Regression was selected for deployment due to its balance between performance and interpretability.

---

## 💡 Example Results

You can run the model using the `predict_price()` function.

```python
predict_price('1st Phase JP Nagar', 1000, 2, 2)
# Output: ₹75.0 Lakhs
```
---


## 🚀 Clone This Repository

```bash
git clone https://github.com/santhosh-labs/zepto-sql-analysis.git
```
---
## 👤 Author

Santhosh S — Data Analyst, Focused on deriving actionable insights, simplifying complex data challenges, and delivering data-driven solutions across domains.

💼 LinkedIn: [Santhosh S](https://www.linkedin.com/in/santhosh-portfolio)  
- Let’s connect professionally and grow your data career


