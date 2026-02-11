# E-commerce User Behavior & Conversion Analysis

## Project Overview

This project analyzes user behavior on an e-commerce platform using industry-standard metrics to generate actionable insights for business operations and conversion optimization.

The goal is to understand traffic patterns, conversion efficiency, user interest, and purchasing behavior to support data-driven operational strategies.

---

## Data Source

The dataset is provided by Alibaba Tianchi Platform:

https://tianchi.aliyun.com/notebook/464175?spm=a2c22.12281897.0.0.209423b72ia1e2

Dataset: `user_action`  

## Time Range
November 18, 2014 – December 18, 2014  
(1-month user behavioral data)

## Data Volume

- 10,000 users  
- 12.25+ million user behavior records  
- 287,000+ products  
- 8,916 product categories

The dataset size is sufficiently large to support statistically meaningful behavioral pattern analysis and robust business insight generation.

---

# Analysis Objectives

### 1. Traffic & Access Pattern Analysis
- Analyze PV (Page Views) and UV (Unique Visitors) across different time dimensions.
- Identify peak access periods to support campaign timing and product exposure optimization.

---

### 2. Conversion Funnel & Product Interest Analysis
- Build a full conversion funnel (PV → Cart → Purchase).
- Evaluate conversion rates at each stage.
- Apply Pareto (80/20) analysis to segment product performance.
- Identify high-interest but low-conversion products.

---

### 3. Consumption Behavior & Retention Analysis
- Analyze purchase frequency.
- Calculate average purchase frequency per paying user.
- Measure repurchase rate and repurchase cycle.
- Understand repeat-buy patterns and customer loyalty.

---

# Key Findings & Business Insights

## 1. Traffic Pattern

- Peak traffic occurs between **20:00–22:00 daily**.
- Highest weekly traffic observed on **Thursday**, followed by Tuesday and Wednesday.
- Significant traffic spike during promotional events (e.g., 12.12).

**Recommendation:**
Optimize product exposure and advertising budget allocation during peak traffic windows to maximize conversion efficiency.

---

## 2. Conversion Funnel Insights

- Overall PV → Purchase conversion rate ≈ **1.04%**.
- Click → Cart conversion ≈ **5.07%**.
- Majority of products have conversion rates below 10%.
- 47% of users rarely complete purchases.
- Cart → Purchase conversion ≈ **20.51%**, indicating strong purchase intent once added to cart.

**Recommendation:**
Improve product recommendation accuracy and optimize low-conversion categories to increase overall funnel efficiency.

---

## 3. Purchase & Retention Behavior

- ~97% of users purchase fewer than 50 times.
- Paying users average **2–2.5 purchases per day**.
- Repurchase rate reaches **87.17%**.
- Repurchase cycle concentrated within **1–5 days**.
- Only ~3% of users exceed 50 purchases (loyal user segment).

**Recommendation:**
Focus on high-frequency users and implement targeted retention campaigns within the first 5 days after purchase.
After 15 days, repurchase probability significantly declines — consider reactivation strategies.

---

# Key Metrics

| Metric | Definition |
|--------|------------|
| PV | Total page views |
| UV | Unique visitors |
| Conversion Rate | Percentage of users completing purchase |
| Repurchase Rate | Percentage of users who purchase again |

---

# Dataset Structure

| Column | Description |
|--------|------------|
| user_id | Unique user identifier (anonymized) |
| item_id | Product identifier (anonymized) |
| behavior_type | User action type (1=Click, 2=Favorite, 3=Add to Cart, 4=Purchase) |
| item_category | Product category |
| time | Timestamp (hour-level precision) |

---

# Analytical Focus

Business question → Behavioral pattern → Conversion impact → Operational strategy

This project emphasizes actionable insights for traffic optimization, funnel improvement, and user retention strategy.
