# Customer Analytics

This project dissects fictitious company sales and customer data using SQL queries and visualizations. 
 
The goal is to understand customer value, cohort dynamics, and churn/retention patterns that drive long-term revenue.

---

## 📊 Query 1 — Customer Lifetime Value (LTV)

**Story:**  
Customers were grouped into segments based on spending percentiles:  
- **High Value**: ≥ 75th percentile  
- **Mid Value**: 25th–75th percentile  
- **Low Value**: ≤ 25th percentile  

**Insight:**  
High-value customers spend dramatically more on average compared to mid- and low-value customers. This shows where most of the company’s lifetime value comes from.

<img src="./Images/1_segment_ltv_mix.png" alt="Average LTV" width="500"/>

**SQL:** See [`SQL Query #1`](./Queries/1_customer_segmentation.sql)  

---

## 📈 Query 2 — Cohort Analysis

**Story:**  
Customers are segmented by their **cohort year** (the year of first purchase). We measure both **customer growth** and **revenue per customer** at acquisition.

**Insight:**  
While the company is acquiring more customers each year, the **revenue per customer is slowly declining**. This suggests we are losing pre-existing customers faster and missing out on maximizing lifetime value.

<img src="./Images/2_cohort_customer_revenue.png" alt="Average LTV" width="500"/>

**SQL:** See [`SQL Query #2`](./Queries/2_cohort_analysis.sql)  

---

## 🔄 Query 3 — Churn & Retention

**Story:**  
We classified customers as **Active** or **Churned** based on whether they purchased in the last 6 months relative to the dataset’s snapshot date.  

**Insight:**  
The majority of customers are **Churned**, highlighting missed opportunities to **re-monetize existing customers**.  
This points toward strategies like re-engagement campaigns, loyalty programs, or personalized marketing to lift retention.

**Visualization:**  
<img src="./Images/3_churned_active_cx.png" alt="Average LTV" width="500"/>

**SQL:** See [`SQL Query #3`](./Queries/3_retension_analysis.sql) 

---

## 🛠 Tech Stack
- **SQL**: Data wrangling, cohort definitions, churn classification  
- **Python (Pandas, Matplotlib)**: Visualization and analysis  
- **GitHub**: Project hosting & version control  

---

## 🚀 Next Steps
- Package this repo with `/sql`, `/images`, and `README.md`  
- Share insights on **LinkedIn**, highlighting:  
  - How SQL is used for real business questions  
  - Key findings on customer value, cohort health, and retention gaps  
  - Potential strategies for improving long-term revenue
