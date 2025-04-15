
# 📊 Regression Analysis, Model Validation and Diagnostics

This project is an academic report developed as part of the *"Introductory Case Studies – Project III: Regression Analysis"* course at **TU Dortmund University** during the **winter term 2023/24**. The study investigates how various factors influence bike rental demand using linear and polynomial regression techniques.

---

## 📌 Project Objectives

- Model the relationship between daily bike rentals and influencing variables  
- Compare linear and polynomial regression models using fit statistics (R², RSE)  
- Apply backward selection using AIC to simplify the model  
- Evaluate regression assumptions: linearity, homoscedasticity, normality, and multicollinearity  
- Interpret the statistical significance of model coefficients

---

## 🗃️ Dataset

The dataset is a cleaned and scaled subset of the UCI Bike Sharing Dataset, with **731 daily records** and **9 variables**, including:

- **Independent Variables**: `mnth`, `weekday`, `workingday`, `weathersit`, `temp`, `atemp`, `hum`, `windspeed`  
- **Target Variable**: `cnt` (daily count of bike rentals)  
- No missing values; appropriate encoding applied for regression compatibility

---

## 📈 Methods Used

- **Modeling**: Multiple Linear Regression, Polynomial Regression  
- **Model Selection**: Backward Elimination using **Akaike Information Criterion (AIC)**  
- **Assumption Checks**:  
  - Linearity and Homoscedasticity: Residual plots  
  - Normality: Q-Q plot  
  - Multicollinearity: Variance Inflation Factor (VIF)  
- **Performance Metrics**: R², Residual Standard Error (RSE), AIC

---

## 🔍 Key Insights

- Polynomial regression improved model performance (R² ↑ from 0.504 to 0.607)  
- Backward selection reduced model complexity by removing 4 variables  
- Final model retained 7 significant predictors and maintained performance  
- Regression diagnostics revealed:  
  - **Non-linearity** and **heteroscedasticity** in residuals  
  - **Multicollinearity** between polynomial terms (e.g., `temp2`, `temp3`)  
  - Violations imply careful interpretation of p-values and confidence intervals is needed

---

## 🛠️ Tools & Technologies

- **Language**: Python 3.12.6  
- **Libraries**: pandas, seaborn, matplotlib, scikit-learn, statsmodels  
- **IDE**: Visual Studio Code
