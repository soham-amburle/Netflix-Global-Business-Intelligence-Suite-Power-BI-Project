# Netflix Global Streaming Intelligence Suite - Subscription Plan Performance Dashboard

**Organization:** Simulated Global Streaming Platform (Inspired by Netflix)  
**Tool:** Power BI  
**Dataset:** Synthetic Streaming Dataset – 2,394 Records  
**Dashboard Focus:** Subscription Plan Adoption, Revenue, and Subscriber Analysis  
**Date:** 14 March 2026  
**Created by:** Soham S. Amburle  

---

## Overview

The **Subscription Plan Performance Dashboard** provides a comprehensive view of how different subscription plans are performing across a simulated global streaming platform. Using a synthetic dataset structured to mirror enterprise-level streaming analytics, this dashboard allows stakeholders to analyze **subscriber distribution, revenue generation, active vs cancelled subscriptions, and plan popularity**.

This dashboard is designed for product managers, executives, and analysts to answer critical questions such as:

- How many subscribers are active vs cancelled?  
- What is the revenue contribution of each subscription plan?  
- How is the subscriber base distributed across countries, regions, and continents?  
- What is the average monthly subscription price across the platform?  
- Which subscription plans are most popular among different user demographics?  

Through KPI cards, interactive slicers, and key visuals, the dashboard provides a **concise yet actionable view** of subscription plan performance.

---

## Business Storyline & Analytical Flow

### 1. Executive KPI Snapshot – KPI Cards

Five KPI cards summarize platform-level metrics:

- **Total Subscribers**  
- **Total Revenue**  
- **Active Subscriptions**  
- **Cancelled Subscriptions**  
- **Average Plan Price**  

These KPIs provide a **quick health check** of the subscription ecosystem, giving executives an immediate understanding of subscriber numbers, revenue, and plan adoption.

---

### 2. Main Visuals

Four key visuals offer insights into subscription performance:

1. **SUBSCRIBERS BY PLAN** – Clustered Column Chart (Total Subscribers per Plan)  
2. **REVENUE BY PLAN** – Area Chart (Revenue Contribution per Plan)  
3. **PLAN DISTRIBUTION** – Donut Chart (Subscriber Proportion per Plan)  
4. **SUBSCRIBERS BY COUNTRY** – Map (Geographic Subscriber Spread)  

These visuals highlight plan popularity, revenue distribution, and geographic adoption trends, enabling clear decision-making for pricing and marketing strategies.

---

### 3. Interactive Slicers

Eight slicers allow dynamic filtering across multiple dimensions:

- Plan Name (`Dim_SubscriptionPlan[PlanName]`)  
- Country (`Dim_Geography[Country]`)  
- Year (`Dim_Time[Year]`)  
- Subscription Status (`Fact_Subscriptions[Status]`)  
- Continent (`Dim_Geography[Continent]`)  
- Region (`Dim_Geography[Region]`)  
- Gender (`Dim_Users[Gender]`)  
- Age (`Dim_Users[Age]`)  

Slicers enable granular exploration, allowing users to **analyze plan performance by geography, time, and demographics**.

---

## Key Takeaways

The dashboard allows stakeholders to:

- Quickly assess subscription plan adoption and revenue contributions  
- Identify high-performing plans and underperforming tiers  
- Monitor active vs cancelled subscription trends  
- Understand geographic and demographic subscriber distribution  
- Support data-driven decisions for pricing, marketing, and retention strategies  

---

## Tools & Data

- **Visualization Tool:** Power BI  
- **Dataset:** Synthetic global streaming dataset  
- **Total Records:** 2,394 rows across 11 tables  
- **Data Model:** Snowflake Schema  
- **Fact Tables:**  
  - Fact_WatchHistory  
  - Fact_Subscriptions  
  - Fact_Ratings  
- **Dimension Tables:**  
  - Dim_Users  
  - Dim_Content  
  - Dim_Time  
  - Dim_Geography  
  - Dim_Genre  
  - Dim_Language  
  - Dim_Device  
  - Dim_SubscriptionPlan  

The dataset was generated using **Mockaroo**, simulating streaming platform scenarios such as **subscription plan adoption, revenue per plan, global geography, and subscriber demographics**.

---

> **Note:** This dashboard is a **portfolio project** and is not affiliated with any real streaming platform. All data is synthetic and created for learning, analysis, and demonstration purposes.

---

**Dashboard and Documentation by SOHAM S. AMBURLE**  
**14 March 2026**
