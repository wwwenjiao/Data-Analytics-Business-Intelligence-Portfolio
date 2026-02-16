# 🚲 London Bike Sharing — Mobility Demand & Network Optimization

## Project Overview

Operational analytics project on ~735,000 bike trips across 800 stations to uncover structural demand patterns, station imbalance, and resource optimization opportunities.

**Data Source:**  

The dataset was obtained from Kaggle:

London Bike Share Usage Dataset  
https://www.kaggle.com/datasets/kalacheva/london-bike-share-usage-dataset

Transport for London (TfL) Open Data  
https://tfl.gov.uk/info-for/open-data-users/our-open-data

---

## Key Insights

- Clear commuter-driven bimodal demand (7–9 AM, 5–6 PM)
- Strong spatial clustering around Hyde Park and central hubs
- Significant net flow imbalance across stations
- All major factors (hour, weekday, station, bike model) statistically significant (ANOVA, p < 0.05)

---

## Station Segmentation (K-Means, k=5)

Stations classified into five operational archetypes:

- Low-volume peripheral stations  
- High-demand outbound hubs  
- Balanced mid-volume stations  
- Inbound-heavy congestion nodes  
- Extreme imbalance hubs  

Segmentation enables differentiated allocation instead of uniform deployment.

---

## Business Impact

- Designed peak-aware redistribution strategy  
- Identified priority high-flow corridors  
- Built cluster-based capacity planning framework  
- Established data-driven mobility decision support model  

---

## Tools

Python | Pandas | Scikit-learn | K-Means | PCA | ANOVA | Matplotlib | Seaborn

