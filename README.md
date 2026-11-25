# Grocery Store Sales & RFM Customer Analytics

An end-to-end data analytics project exploring grocery store transaction data using **Python**, **SQL (SQLite)**, **Matplotlib/Seaborn**, and **Plotly** to uncover category performance, monthly sales trends, spend distributions, and RFM customer segments.

## Project Overview
Retail and grocery businesses rely on repeat footfall, staple item volume, and timely customer retention. This project analyzes store transactions to answer:
* Which product categories drive revenue and profit margins?
* How does monthly revenue trend across the year?
* How are customer monetary values distributed, and are there high-value outliers?
* Which customer segments contribute the most revenue, and which ones need retention or win-back actions?

## Dataset & Methodology
* **Data & SQL Layer:** Queried transaction records in SQLite (`run_query` helper) to aggregate category revenue, profit, profit margin percentage, and monthly revenue trends.
* **RFM Segmentation:** Scored customers on **Recency** (days since last purchase), **Frequency** (number of purchases), and **Monetary** value (total spend), grouping them into segments such as *Champions*, *Loyal Customers*, *At-Risk Customers*, *Potential Loyalists*, *Hibernating*, and *Recent Customers*.
* **Visualizations:** Built category and monthly trend charts with Matplotlib/Seaborn, alongside interactive Plotly bar charts, box plots, and a revenue-vs-recency treemap.
* **Outlier Handling:** Used box plots to inspect monetary spend distributions across segments. High-spend upper outliers (such as around ₹10k in *Potential Loyalists*) represent genuine larger/bulk orders rather than data errors, so they were retained in the analysis.

## Key Takeaways
* **Category Performance:** **Staples & Grains** leads total revenue by a wide margin (₹6,61,065), while categories like **Personal & Household** and **Snacks & Beverages** offer stronger profit margins—making staples key for footfall and cross-selling/bundles useful for basket size.
* **Monthly Trend:** Sales dip in February, pick up in March, peak in July, and finish strong toward December, showing stronger momentum in the second half of the year.
* **Customer Segments & Retention:** **Champions** and **Loyal Customers** drive the largest share of revenue, while **At-Risk Customers** and **Hibernating** buyers hold substantial revenue with higher recency—making timely follow-ups, win-back offers, and second-purchase nudges for **Recent Customers** high-impact priorities.

## Tools & Libraries
* **Language & Environment:** Python, Jupyter Notebook / JupyterLab
* **Database:** SQLite (`sqlite3`)
* **Data & Visualization:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`

## How to Run Locally
1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd <your-repo-folder>