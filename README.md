# Customer Analytics Project (SQL + Visualization)

This project dissects fictitious company sales and customer data using SQL queries and visualizations. 
 
The goal is to understand customer value, cohort dynamics, and churn/retention patterns that drive long-term revenue.

---

## 📊 Query 1 — Customer Segmentation by Lifetime Value (LTV)

**Story:**  
Customers were grouped into segments based on spending percentiles:  
- **High Value**: ≥ 75th percentile  
- **Mid Value**: 25th–75th percentile  
- **Low Value**: ≤ 25th percentile  

**Insight:**  
High-value customers spend dramatically more on average compared to mid- and low-value customers. This shows where most of the company’s lifetime value comes from.

**SQL:** See [`sql/query_01_customer_segmentation.sql`](./sql/query_01_customer_segmentation.sql)  

**Visualizations:**  
- Average LTV by segment:  
  ![Average LTV](images/q1_avg_ltv_by_segment.png)  
- Customer distribution across segments:  
  ![Customer Distribution](images/q1_customer_count_distribution.png)  

---

## 📈 Query 2 — Cohort Analysis (First Purchase Year)

**Story:**  
Customers are segmented by their **cohort year** (the year of first purchase). We measure both **customer growth** and **revenue per customer** at acquisition.

**Insight:**  
While the company is acquiring more customers each year, the **revenue per customer is slowly declining**. This suggests we are losing pre-existing customers faster and missing out on maximizing lifetime value.

**SQL:** See [`sql/query_02_cohort_analysis.sql`](./sql/query_02_cohort_analysis.sql)  

**Visualizations:**  
- Total customers by cohort year:  
  ![Total Customers](images/q2_total_customers_by_cohort.png)  
- Revenue per customer by cohort year:  
  ![Revenue per Customer](images/q2_revenue_per_customer_by_cohort.png)  

---

## 🔄 Query 3 — Churn & Retention by Cohort

**Story:**  
We classified customers as **Active** or **Churned** based on whether they purchased in the last 6 months relative to the dataset’s snapshot date.  

**Insight:**  
The majority of customers are **Churned**, highlighting missed opportunities to **re-monetize existing customers**.  
This points toward strategies like re-engagement campaigns, loyalty programs, or personalized marketing to lift retention.

**SQL:** See [`sql/query_03_churn_by_cohort.sql`](./sql/query_03_churn_by_cohort.sql)  

**Visualization:**  
- Retention mix (Active vs. Churned) by cohort:  
  ![Retention Mix](images/q3_retention_mix_100pct.png)  

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
