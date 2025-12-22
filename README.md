# 🛒 RFM Customer Segmentation & Actionable Insights
![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Pandas](https://img.shields.io/badge/Library-Pandas-green)
![Plotly](https://img.shields.io/badge/Visualization-Plotly-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Overview
This project performs a comprehensive **Customer Segmentation Analysis** using the **RFM (Recency, Frequency, Monetary)** technique on the *Online Retail II* dataset. 

Beyond standard segmentation, this project includes a **Business Action Layer** that automatically generates strategic marketing recommendations based on the Pareto Principle (focusing on the most impactful segments).

## 💼 Business Problem
A retail company wants to segment its customers to optimize marketing costs and increase revenue. Instead of mass marketing, they need a data-driven approach to:
* Identify **Champions** (Most valuable customers).
* Re-activate **Hibernating** customers.
* Prevent churn in **At Risk** groups.

## 🛠️ Key Features & Methodology
The project follows a modular, functional pipeline architecture:

1.  **Data Preprocessing Pipeline:** * Automated outlier detection and removal.
    * Handling of returned transactions (Invoice codes containing 'C').
    * Data type standardization.
2.  **RFM Calculation Engine:**
    * Dynamic calculation of Recency, Frequency, and Monetary metrics.
    * Scoring customers on a 1-5 scale using `qcut`.
3.  **Advanced Segmentation:**
    * Regex-based mapping to categorize customers into 10 distinct segments (e.g., *Loyal Customers, Potential Loyalists, Need Attention*).
4.  **Interactive Visualization:**
    * **Treemap:** To visualize the market share of each segment.
    * **3D/2D Scatter Plots:** To analyze the correlation between Recency and Frequency using Plotly.
5.  **Automated Action Plan:**
    * A rule-based system that suggests specific marketing strategies (Upsell, Cross-sell, Churn Prevention) for the top 3 segments.

## 📊 Visuals & Insights
*(Note: Interactive charts are generated using Plotly)*

### 1. Segment Distribution (Treemap)
Visualizing the dominance of "Hibernating" vs "Champions" segments to understand customer retention health.

### 2. Recency vs Frequency Matrix
Analyzing customer positioning to identify potential loyalists moving towards the "Champions" zone.

## 🚀 How to Run
1.  Clone the repository:
    ```bash
    git clone https://github.com/kaanhitay/CRM-Analytics-Customer-Segmentation.git
    ```
2.  Install dependencies:
    ```bash
    pip install pandas plotly openpyxl
    ```
3.  Run the notebook:
    ```bash
    jupyter notebook RFM_Customer_Segmentation_Analysis.ipynb
    ```

## 📈 Results (Executive Summary)
The analysis identified critical segments requiring immediate attention:
* **Champions:** High engagement. Strategy: *Reward & Advocate Programs.*
* **Hibernating:** Low engagement. Strategy: *Aggressive Discounting for Re-activation.*
* **At Risk:** Declining activity. Strategy: *Personalized Outreach.*

---
*Created by Serhat Kaan Hitay*
