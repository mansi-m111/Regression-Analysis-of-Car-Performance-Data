# 📊 Regression Analysis of Car Performance Data

![Made with Python](https://img.shields.io/badge/Made%20with-Python-blue?logo=python)

This project performs a comprehensive **regression analysis** on classic car performance data to explore how various vehicle attributes influence **fuel efficiency** (measured in miles per gallon, mpg). The goal is to demonstrate how statistical modeling can uncover actionable insights into automotive design and performance.

---

## 📌 Project Overview

- **Dataset**: `mtcars` (Motor Trend Car Road Tests)
- **Observations**: 32 cars
- **Variables**: 11 numeric features including:
  - `mpg`, `cyl`, `disp`, `hp`, `drat`, `wt`, `qsec`, `vs`, `am`, `gear`, `carb`

This case study uses Python and `statsmodels` to build, interpret, and compare multiple linear regression models. It includes data preprocessing, exploratory analysis, model construction, diagnostics, and interpretation of results.

---

## 🎯 Objectives

- **Feature Exploration**  
  Understand how attributes like weight, horsepower, and engine size impact fuel efficiency.

- **Model Building**  
  Construct and compare regression models to identify the best predictors of `mpg`.

- **Statistical Interpretation**  
  Evaluate model fit, check assumptions, and interpret coefficients for data-driven insights.

---

## 🧰 Tools & Technologies

- **Language**: Python
- **Libraries**: `pandas`, `numpy`, `statsmodels`, `seaborn`, `matplotlib`

---

## 🧪 Methodology

### 🟠 Data Preparation
- Loaded and cleaned the `mtcars` dataset
- Explored distributions and summary statistics
- Checked for missing values and outliers

### 🟠 Regression Modeling
- Built multiple linear regression models:
  - Full model with all predictors
  - Stepwise models with selected features
- Evaluated models using:
  - R-squared and Adjusted R-squared
  - AIC and BIC
  - F-statistics and p-values
- Interpreted coefficients and confidence intervals

### 🟠 Diagnostics & Validation
- Checked for:
  - Normality of residuals
  - Homoscedasticity
  - Multicollinearity (VIF)
- Plotted residuals and influence diagnostics

---

## 📊 Key Findings

- **Weight (`wt`)** and **cylinders (`cyl`)** are strong negative predictors of fuel efficiency.
- **Horsepower (`hp`)** and **displacement (`disp`)** also negatively impact mpg, though their significance varies across models.
- **Transmission (`am`)**: Manual cars tend to have higher mpg, but the effect size depends on the model.
- Best models explain ~83–87% of variance in mpg (R² ≈ 0.83–0.87).
- **Multicollinearity** among predictors like `cyl`, `hp`, and `disp` affects coefficient stability.

