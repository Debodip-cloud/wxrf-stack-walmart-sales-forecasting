# WXRF-Stack: Walmart Sales Forecasting Using Hybrid Ensemble Learning

## Overview

WXRF-Stack is a hybrid machine learning framework developed for retail sales forecasting using Walmart sales data. The project combines Random Forest and XGBoost through a stacking architecture, with Linear Regression acting as a meta-learner to generate final predictions.

The objective of the project is to improve forecasting accuracy while maintaining model interpretability. In addition to predictive modelling, the project includes exploratory data analysis, feature engineering, model comparison, cross-validation, feature importance analysis, and SHAP-based explainability.

This project was also developed as part of an academic research study on machine learning applications in retail analytics.

---

## Business Problem

Retail organizations rely on accurate sales forecasts to support:

* Inventory management
* Supply chain planning
* Workforce scheduling
* Promotional campaign planning
* Strategic decision-making

Poor forecasts can lead to stock shortages, excess inventory, higher operational costs, and reduced customer satisfaction.

The aim of this project is to develop a forecasting framework that can help retailers predict future sales more accurately and make better business decisions.

---

## Dataset

**Dataset:** Walmart Sales Dataset

The dataset contains weekly sales records from Walmart stores together with operational and economic variables such as:

* Store ID
* Weekly Sales
* Holiday Flag
* Temperature
* Fuel Price
* Consumer Price Index (CPI)
* Unemployment Rate
* Date

Additional time-based features were created through feature engineering, including:

* Year
* Month
* Week Number
* Day

---

## Project Workflow

### 1. Data Preprocessing

* Data cleaning
* Duplicate removal
* Date conversion
* Feature engineering
* Train-test split

### 2. Exploratory Data Analysis

* Sales trend analysis
* Feature distribution analysis
* Correlation analysis

### 3. Machine Learning Models

The following models were evaluated:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor
4. XGBoost Regressor
5. WXRF-Stack (Proposed Framework)

### 4. Explainable AI

* Feature Importance Analysis
* SHAP Explainability

### 5. Model Evaluation

Performance was evaluated using:

* R² Score
* Adjusted R²
* MAE
* RMSE
* MAPE
* 5-Fold Cross Validation

---

## WXRF-Stack Framework

The proposed framework consists of:

Random Forest → Base Learner

XGBoost → Base Learner

Linear Regression → Meta Learner

Final Prediction → Weekly Sales Forecast

The stacking architecture combines the strengths of both Random Forest and XGBoost to improve predictive performance.

---

## Results

| Model             | R² Score   |
| ----------------- | ---------- |
| Linear Regression | 0.1306     |
| Decision Tree     | 0.8234     |
| Random Forest     | 0.9065     |
| XGBoost           | 0.9474     |
| WXRF-Stack        | **0.9536** |

### Additional Validation

| Metric       | Value  |
| ------------ | ------ |
| R²           | 0.9536 |
| Adjusted R²  | 0.9571 |
| MAPE         | 8.95%  |
| Mean CV R²   | 0.9457 |
| CV Std. Dev. | 0.0293 |

The results demonstrate that WXRF-Stack achieved the best forecasting performance among all evaluated models.

---

## Key Findings

* Store-level characteristics were the most important predictors of weekly sales.
* CPI had a stronger influence on forecasts than temperature-related variables.
* The hybrid stacking approach improved predictive accuracy beyond individual machine learning models.
* SHAP analysis improved model interpretability and provided insights into the factors driving sales predictions.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* SHAP
* Jupyter Notebook
* Kaggle

---

## Repository Structure

```text
├── data/
├── notebooks/
│   └── walmart_sales_forecasting.ipynb
├── figures/
│   ├── sales_trend.png
│   ├── feature_importance.png
│   ├── actual_vs_predicted.png
│   ├── residual_plot.png
│   └── shap_summary.png
├── paper/
│   └── wxrf_stack_research_paper.pdf
├── README.md
```

---

## Research Contribution

This study proposes a hybrid Random Forest–XGBoost stacking framework for retail sales forecasting and demonstrates that combining ensemble learning with explainable AI techniques can improve both predictive performance and business interpretability.

---

## Author

**Debodip Chowdhury**

MSc Financial Technology with Data Science

University of Bristol

Interests: Data Science, Machine Learning, Financial Technology, Explainable AI, Retail Analytics
