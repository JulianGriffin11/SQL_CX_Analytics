#  💳 SQL Segments: Retail Customer Analytics 💳

---

## 📖 Background
This project was built by following Luke Barousse's structured SQL Intermediate guide on a simulated retail dataset.  

The intent was to replicate how a real company might explore customer lifetime value, acquisition cohorts, and churn trends — turning raw transactions into actionable business insights. By combining SQL with visualization, the project demonstrates end-to-end analytical thinking: from query design to storytelling.

---

## 📊 Query 1 — Customer Lifetime Value (LTV)

**Goal:** Understand who our **low, mid,** and **high value customers** are based on spending, and determine their consumer LTV.

**Process:**  
1. Customers were grouped into 1 of 3 segments based on spending percentiles:  
   - **High Value**: ≥ 75th percentile  
   - **Mid Value**: 25th–75th percentile  
   - **Low Value**: ≤ 25th percentile  
2. Aggregated the segments to calculate how much they spent on average over all of their unique purchases.

**Insight:**  
High-value customers spend dramatically more on average compared to mid and low-value customers. This shows where most of the company’s lifetime value comes from.

<br>

<img src="./Images/1_segment_ltv_mix.png" alt="Average LTV" width="500"/>

🚀 [Dive deeper into my 1st SQL Query](./Queries/1_customer_segmentation.sql) 🚀

---

## 📈 Query 2 — Cohort Analysis

**Goal:** Group customers by **Cohort Year** (first purchase year) to determine what percentage of customers are new every year.

**Process:**  
1. Customers were aggregated by their year of first purchase.  
2. **Customer growth** and **Revenue Per Customer** were calculated and compared in each year.

**Insight:**  
While the company is acquiring more customers each year, the **revenue per customer is slowly declining**. This suggests we are losing pre-existing customers faster and missing out on maximizing lifetime value.

<br>

<img src="./Images/2_cohort_customer_revenue.png" alt="Revenue per Customer" width="500"/>

🚀 [Dive deeper into my 2nd SQL Query](./Queries/2_cohort_analysis.sql) 🚀

---

## 🔄 Query 3 — Churn & Retention

**Goal:** Determine which percentage of our customers are **Churned** (haven’t purchased in last 6 months) and which percentage are **Active** (have purchased in last 6 months).

**Process:**  
1. Each customer's last purchase date was queried.  
2. Classified as **Active** or **Churned** based on whether they purchased in the last 6 months relative to the dataset’s snapshot date.  

**Insight:**  
The majority of customers are **Churned**, highlighting missed opportunities to **re-monetize existing customers**. This points toward strategies like re-engagement campaigns, loyalty programs, or personalized marketing to lift retention.

<br>

<img src="./Images/3_churned_active_cx.png" alt="Retention Mix" width="500"/>

🚀 [Dive deeper into my 3rd SQL Query](./Queries/3_retension_analysis.sql) 🚀

---

## 🛠 Tech Stack
- **SQL**: Views & CTEs to define complex queries  
- **Chat GPT**: Generating visualizations  
- **GitHub**: Project hosting & organization  

---

## 🚀 What I Learned
- How to **design queries around business problems** (segmentation, cohorts, churn).  
- How to **combine SQL with visual storytelling** so insights are accessible to non-technical audiences.

---

✨ Click the heading links to dive deeper into each project! 🚀  

- Check out some of my other work:  
  - [📊 Excel Projects](https://github.com/JulianGriffin11/Excel_Projects)  
  - [📘 R Projects](https://github.com/JulianGriffin11/R_Projects)  

Sincerely,  
Julian Griffin 
