# Marketing-Analytics-HW3
# Telco Customer Churn & Survival Analysis

## Project Overview
This repository contains a comprehensive Survival Analysis of telecom customer churn using Accelerated Failure Time (AFT) models. The objective is to understand the factors driving customer churn, estimate Customer Lifetime Value (CLV), and propose an actionable, data-driven annual retention budget.

## Repository Contents
* `survival_analysis.py` / `notebook.ipynb` - The primary codebase handling data preprocessing, AFT modeling, feature selection, and CLV calculations.
* `Report.md` - A business report detailing the findings, interpretations of risk factors, and retention strategies.
* `requirements.txt` - Dependencies required to run the environment.
* `telco.csv` - The telecom dataset (ensure this is in the same directory as the script).

## Methodology
1. **Parametric Modeling**: Weibull, Log-Normal, and Log-Logistic AFT models were built and compared using AIC.
2. **Feature Selection**: The best-performing model was optimized by retaining only statistically significant predictors.
3. **CLV Calculation**: Discounted cash flow logic was applied to the predicted survival curves to compute individual and segment-based CLV.
4. **Retention Budgeting**: At-risk customers were identified by calculating conditional survival probabilities for the upcoming year to formulate a target retention budget.
