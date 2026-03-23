# Global Streaming Intelligence Suite – Customer Churn Analysis

**Organization:** Netflix (Simulated Streaming Analytics Model)  
**Tool:** Power BI  
**Dataset:** Synthetic Global Streaming Dataset – ~2,394 Records  
**Dashboard Focus:** Customer Churn, Retention Risk, and Subscription Behavior  
**Date:** 23 March 2026  
**Created by:** Soham S. Amburle  

---

## Overview

The **Customer Churn Analysis Dashboard** provides a comprehensive view of subscriber retention and cancellation behavior across a global streaming platform.

Built using a synthetic dataset and a snowflake schema data model, this dashboard enables stakeholders to identify **churn patterns, revenue impact, and high-risk customer segments**.

This dashboard answers critical business questions:

* What is the overall churn rate of the platform?
* How many users are cancelling vs staying active?
* Which subscription plans experience the highest churn?
* Which countries contribute most to churn?
* Which user segments are more likely to churn?

Through KPI cards, charts, and slicers, the dashboard delivers an **interactive and decision-focused view of customer retention and churn drivers**.

---

## Business Storyline & Analytical Flow

### 1. Churn Snapshot – KPI Cards

Eight KPI cards provide a high-level overview:

* **Total Subs**
* **Active Subs**
* **Cancelled Subs**
* **Churn Rate (%)**
* **Avg Monthly Price**
* **Revenue Lost**
* **ARPU**
* **Churned Users**

These KPIs help stakeholders quickly assess **customer retention health, financial impact, and churn magnitude**.

---

### 2. Main Analytical Visuals

Five visuals provide deeper churn insights:

1. **CHURN BY PLAN** – Clustered Column Chart (Unit: Subscribers)  
2. **CHURN BY COUNTRY** – Map (Unit: Subscribers)  
3. **CHURN BY PLAN & STATUS** – Stacked Bar Chart (Unit: Subscribers)  
4. **CHURN BY AGE GROUP** – Area Chart (Unit: Subscribers)  
5. **CHURN BY GENDER** – Donut Chart (Unit: %)  

These visuals highlight **where churn occurs and which segments are most at risk**.

---

### 3. Interactive Slicers

Eight slicers enable dynamic filtering:

* Subscription Plan (`Dim_SubscriptionPlan[PlanName]`)
* Continent (`Dim_Geography[Continent]`)
* Country (`Dim_Geography[Country]`)
* Year (`Dim_Time[Year]`)
* Gender (`Dim_Users[Gender]`)
* Age Group (`Dim_Users[Age Group]`)
* Status (`Fact_Subscriptions[Status]`)
* Device Type (`Dim_Device[DeviceType]`)

These slicers allow exploration across **geography, demographics, and subscription attributes**.

---

## Key Takeaways

This dashboard enables stakeholders to:

* Monitor churn rate and retention performance  
* Identify high-churn subscription plans  
* Detect geographic regions with high churn  
* Understand which demographic segments are at risk  
* Quantify revenue loss due to cancellations  
* Support targeted retention and pricing strategies  

---

## Tools & Data

* **Visualization Tool:** Power BI  
* **Dataset:** Synthetic global streaming dataset  
* **Record Count:** ~2,394 rows  
* **Data Model:** Snowflake Schema  
* **Purpose:** Customer churn and retention analytics for BI portfolio  

---

> **Note:** This project is not affiliated with Netflix. All data is synthetic and created solely for educational and portfolio purposes.

---

**Dashboard and Documentation by SOHAM S. AMBURLE**  
**23 March 2026**
