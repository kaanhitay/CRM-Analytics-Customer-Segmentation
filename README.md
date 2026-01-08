# RFM Customer Segmentation & Actionable Insights
Customer segmentation using RFM (Recency, Frequency, Monetary) on the Online Retail II dataset, with a simple rule-based action layer for business recommendations.

## Project Overview
This project performs customer segmentation using the RFM technique on the Online Retail II dataset.  
In addition to segmentation, it generates suggested marketing actions for the most common customer segments.

## Business Problem
A retail company wants to segment customers to optimize marketing efforts and increase revenue by:
- Identifying high-value customers (Champions)
- Re-activating inactive customers (Hibernating)
- Preventing churn in declining groups (At Risk)

## Key Features & Methodology
- **Data Preprocessing**
  - Removes missing Customer IDs
  - Filters cancelled invoices (invoices starting with `C`)
  - Filters invalid quantity/price entries
  - Feature engineering: `TotalPrice = Quantity * Price`
- **RFM Metrics**
  - Recency: days since last purchase
  - Frequency: number of unique invoices
  - Monetary: total spend
- **Scoring & Segmentation**
  - Scores customers on a 1–5 scale using quantiles (`qcut`)
  - Regex-based mapping into common RFM segments (e.g., Champions, Loyal Customers, At Risk)
- **Visualization (Plotly)**
  - Treemap for segment distribution
  - Recency vs Frequency scatter plot (log scale)
- **Action Plan**
  - Prints suggested actions for the top 3 most frequent segments

## How to Run
```bash
git clone https://github.com/kaanhitay/CRM-Analytics-Customer-Segmentation.git
pip install pandas plotly openpyxl
jupyter notebook RFM_Customer_Segmentation_Analysis.ipynb

