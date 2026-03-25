
# Olist E-Commerce Sales Analysis

Sales strategy analysis built on Olist's publicly released transaction data — 100K orders, 9 tables, 2 years of Brazilian e-commerce activity.

---

## Business Questions
1. What was the best month for sales?
2. Which state had the highest revenue?
3. What is the best time of day to advertise?
4. What are the best-selling product categories?
5. What products are most often bought together?
6. Who are the most valuable customers? (RFM Segmentation)
7. How do review scores correlate with sales performance?
8. How did the business grow year-over-year?
9. What payment methods do customers prefer?
10. How reliable is the delivery performance?

---

## Dataset
- **Source:** [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
- **Period:** September 2016 – October 2018
- **Orders:** 99,441
- **Tables:** 9 relational CSVs

---

## Tools Used

![Jupyter](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) ![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white)

- **Jupyter Notebook** is used as the IDE via Google Colab.
- **Pandas** is used for data handling, cleaning, and preprocessing across 9 relational tables.
- **Matplotlib and Seaborn** are used for static visualizations and distribution plots.
- **Plotly** is used for interactive charts.
- **Mlxtend** is used for market basket analysis with the Apriori algorithm.

For more details, please go through the Jupyter Notebook attached above.

---

## Analysis & Key Findings

### Best Month for Sales
November 2017 was the peak revenue month, driven by Black Friday. Sales spike consistently in Q4, suggesting inventory and promotions should be concentrated in the Oct–Nov window.

![Monthly Revenue](charts/01_monthly_revenue.png)

---

### Revenue by State
São Paulo dominates with ~38% of total revenue — nearly 3x Rio de Janeiro in second place. Logistics investment and same-day delivery expansion should prioritise SP first.

![Revenue by State](charts/02_revenue_by_state.png)

---

### Best Time to Advertise
Order volume peaks at 16:00 and is highest on Mondays. The optimal window for paid advertising is 15:00–17:00 on weekdays. Weekend campaigns show significantly lower order activity.

![Orders by Hour](charts/03_orders_by_hour.png)

---

### RFM Customer Segmentation
RFM analysis reveals that most customers only purchase once — average frequency is 1.0 across nearly every segment. The 17,411 "Cannot Lose Them" customers haven't bought in over a year but previously spent well. A targeted re-engagement campaign here is the highest-leverage retention move.

![RFM Segments](charts/04_rfm_segments.png)

---

### Year-over-Year Growth
Revenue grew +22.1% and orders grew +21.5% from 2017 to 2018. The near-identical growth rates mean average order value stayed flat — Olist scaled by acquiring more customers, not by charging more.

![YoY Comparison](charts/05_yoy_comparison.png)

---

### Delivery Performance
92.4% of orders arrive on time. More notably, Olist estimates 23 days but delivers in 12 on average — an 11-day buffer that directly explains the high 5-star review rate. Advertising realistic delivery times could be a strong competitive differentiator.

![Delivery Performance](charts/06_delivery_performance.png)

---

## Conclusion
- **Best month:** November 2017 — Black Friday peak (BRL 1,153,364)
- **Top state:** São Paulo — 38% of total revenue
- **Best ad window:** 15:00–17:00 on Mondays
- **Top category by revenue:** Health & Beauty (avg BRL 130)
- **Top category by volume:** Bed & Bath (10,953 units)
- **YoY growth:** +22% revenue and orders
- **Retention problem:** avg purchase frequency of 1.0 across all segments
- **Delivery edge:** delivers 11 days faster than promised — drives 5-star reviews