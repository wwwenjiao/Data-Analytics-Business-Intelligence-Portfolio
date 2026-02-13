# HR Analytics: Employee Attrition Prediction

## 1. Project Overview

This project develops an end-to-end employee attrition prediction system to identify high-risk employees, uncover structural turnover drivers, and translate predictive insights into actionable HR strategies.

The objective is not only to predict attrition but to transform model outputs into interpretable, business-ready decision support.

---

## 2. Data Source

The dataset used in this project is the publicly available **HR Analytics Employee Attrition Dataset**, commonly shared on Kaggle for workforce analytics and machine learning practice.

- Source: Kaggle – HR Analytics Dataset (https://www.kaggle.com/mizanhadi/hr-employee-data-visualisation/data?select=HR_comma_sep.csv) 
- Type: Structured tabular employee data  
- Use Case: Educational and analytical modeling  

The dataset contains anonymized employee records.

---

## 3. Dataset Structure

File: `HR_comma_sep.csv`

### Dataset Size
- ~15,000 employee records  
- 9 feature variables  
- 1 binary target variable  

---

## 4. Variable Description

| No | Feature Name              | Type    | Description |
|----|---------------------------|---------|-------------|
| 1  | satisfaction_level        | Float   | Employee satisfaction score (0–1 scale) |
| 2  | last_evaluation           | Float   | Last performance evaluation score (0–1 scale) |
| 3  | number_project            | Integer | Number of projects completed |
| 4  | average_monthly_hours     | Integer | Average monthly working hours |
| 5  | time_spend_company        | Integer | Years spent at the company |
| 6  | work_accident             | Integer | Work accident history (0 = No, 1 = Yes) |
| 7  | promotion_last_5years     | Integer | Promotion in last 5 years (0 = No, 1 = Yes) |
| 8  | department (sales)        | String  | Department name |
| 9  | salary                    | String  | Salary level (low / medium / high) |
| 10 | left                      | Integer | Attrition status (0 = Active, 1 = Attrited) |

---

## 5. Analytical Framework

### 5.1 Exploratory Data Analysis (EDA)

- Attrition distribution analysis  
- Correlation heatmap  
- Department-level turnover comparison  
- Salary structure analysis  
- Tenure-based attrition rate curve  
- Promotion vs attrition comparison  

Key Insight:
- 3–4 years tenure represents a high-risk attrition window.
- Satisfaction level is the strongest turnover indicator.

---

### 5.2 Predictive Modeling

**Baseline Model**
- Logistic Regression  
- ROC-AUC ≈ 0.84  

**Strong Model**
- Random Forest  
- ROC-AUC ≈ 0.99  
- Validated with 5-fold cross-validation  

**Risk-Based Intervention Strategy**
- Top 10% predicted risk threshold  
- 100% precision  
- 43% attrition capture rate  

---

## 6. Model Interpretation

SHAP (SHapley Additive Explanations) was applied to:

- Identify dominant attrition drivers  
- Capture non-linear feature interactions  
- Explain individual employee risk profiles  

Primary Drivers:
- Low satisfaction level  
- Mid-career stagnation (3–4 years tenure)  
- Workload imbalance  
- Promotion gap  
- Salary concentration effects  

---

## 7. Business Implications

- Attrition is structurally predictable  
- Behavioral signals outweigh departmental impact  
- Early-career intervention programs are critical  
- Promotion transparency reduces turnover risk  
- Predictive modeling enables proactive HR decision-making  

---

## 8. Tech Stack

- Python  
- Pandas / NumPy  
- Scikit-learn  
- SHAP  
- Matplotlib / Seaborn  

---

## 9. Future Improvements

- Temporal validation split  
- Cost-sensitive optimization  
- Deployment-ready risk dashboard  
- Uplift modeling for intervention evaluation  

---

## Project Summary

Employee attrition is not random — it follows identifiable behavioral patterns.  
This project demonstrates how interpretable machine learning can convert workforce data into actionable retention strategies.
