# HR Analytics: Attrition Prediction & Workforce Insights

## 1. Project Overview

This project develops an end-to-end employee attrition prediction system, combining exploratory analysis, predictive modeling, model interpretation, and business strategy translation.

The goal is not only to predict employee turnover but to transform predictive signals into actionable HR decision support.

---

## 2. Objectives

- Identify key drivers of employee attrition
- Quantify workforce risk patterns
- Build interpretable predictive models
- Design data-driven retention strategies

---

## 3. Dataset Description

The dataset includes 10 employee-related variables such as:

- satisfaction_level
- last_evaluation
- number_project
- average_monthly_hours
- time_spend_company
- work_accident
- promotion_last_5years
- department
- salary
- left (target variable)

---

## 4. Methodology

### 4.1 Exploratory Data Analysis (EDA)

- Attrition distribution analysis
- Tenure-based risk window identification
- Salary structure analysis
- Promotion vs attrition comparison
- Correlation analysis

Key insight: 3–4 years tenure represents a critical attrition spike.

---

### 4.2 Predictive Modeling

Baseline Model:
- Logistic Regression (ROC-AUC = 0.84)

Strong Model:
- Random Forest (ROC-AUC = 0.99)
- 5-fold Cross Validation confirmed stability

Risk Strategy:
- Top 10% risk threshold achieves:
  - 100% precision
  - 43% attrition capture rate

---

### 4.3 Model Interpretation

SHAP was used to:

- Identify dominant attrition drivers
- Analyze non-linear relationships
- Explain individual employee risk profiles

Primary drivers:
- Low satisfaction
- Mid-career stagnation
- Workload imbalance
- Promotion gap

---

## 5. Key Findings

- Job satisfaction is the strongest predictor of attrition
- Mid-career employees (3–4 years tenure) show highest turnover risk
- Behavioral factors outweigh department effects
- Compensation structure is skewed toward low-salary employees
- Attrition patterns are highly predictable and structurally driven

---

## 6. Business Impact

- Enables proactive retention monitoring
- Supports targeted HR interventions
- Converts prediction into decision support
- Provides interpretable AI for workforce strategy

---

## 7. Tech Stack

- Python
- Pandas / NumPy
- Scikit-learn
- SHAP
- Matplotlib / Seaborn

---

## 8. Future Improvements

- Temporal validation split
- Cost-sensitive optimization
- Deployment-ready risk dashboard
- Uplift modeling for intervention effectiveness

