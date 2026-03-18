# Global Streaming Intelligence Suite – Customer Demographics Dashboard

**Organization:** Netflix (Simulated Global Streaming Model)
**Tool:** Power BI
**Dataset:** Synthetic Global Streaming Dataset – ~2,394 Records
**Dashboard Focus:** User Demographics Analysis across Age, Gender, Geography, and Subscription Plans
**Date:** 15 March 2026
**Created by:** Soham S. Amburle

---

## Overview

The **Customer Demographics Dashboard** provides a comprehensive view of the user base of a simulated global streaming platform inspired by Netflix. Built using a synthetic dataset and a snowflake schema data model, this dashboard enables analysts and decision-makers to explore **who the users are**, how they are distributed across **age groups, gender, geography, and subscription plans**, and how the user base evolves over time.

This dashboard is designed to answer key business questions such as:

* What is the demographic composition of the user base?
* How are users distributed across age groups and gender?
* Which regions and countries have the highest user concentration?
* What subscription plans are most popular among different user segments?
* How diverse is the global user base?

Through KPI indicators, demographic charts, maps, and slicers, the dashboard provides an **interactive and intuitive user profiling experience**.

---

## Business Storyline & Analytical Flow

### 1. Demographic KPI Snapshot – KPI Cards

Six KPI cards provide a quick overview of the user base:

* **Total Users**
* **Average Age**
* **Male Users**
* **Female Users**
* **Total New Users (YTD)**
* **Average User Tenure (Days)**

These KPIs offer a **high-level snapshot of user scale and composition**.

---

### 2. Core Demographic Visuals

The dashboard includes key visuals to analyze user distribution:

1. **AGE DISTRIBUTION** – Clustered Column Chart
2. **GENDER DISTRIBUTION** – Pie Chart
3. **USERS BY COUNTRY** – Map Visualization
4. **USERS BY SUBSCRIPTION PLAN** – Donut Chart
5. **AGE VS GENDER DISTRIBUTION** – Stacked Column Chart

These visuals allow users to explore demographic patterns across multiple dimensions.

---

### 3. Interactive Slicers

Eight slicers enable dynamic filtering:

* Gender (`Dim_Users[Gender]`)
* Age (`Dim_Users[Age]`)
* Country (`Dim_Geography[Country]`)
* Region (`Dim_Geography[Region]`)
* Continent (`Dim_Geography[Continent]`)
* Signup Year (`Dim_Time[Year]`)
* Signup Month (`Dim_Time[Month]`)
* Subscription Plan (`Dim_SubscriptionPlan[PlanName]`)

These slicers provide **flexibility to drill down into specific demographic segments**.

---

## Key Takeaways

This dashboard enables stakeholders to:

* Understand the composition of the global user base
* Identify dominant age groups and gender distribution
* Analyze geographic concentration of users
* Evaluate subscription plan preferences among users
* Segment users effectively for targeted strategies

---

## Tools & Data

* **Visualization Tool:** Power BI
* **Dataset:** Fully synthetic streaming dataset
* **Record Count:** ~2,394 rows across all tables
* **Data Model:** Snowflake Schema
* **Tables Used:**

  * Fact Tables: Fact_WatchHistory, Fact_Subscriptions, Fact_Ratings
  * Dimension Tables: Dim_Users, Dim_Content, Dim_Time, Dim_Geography, Dim_Genre, Dim_Language, Dim_Device, Dim_SubscriptionPlan

---

> **Note:** This project is not affiliated with Netflix. All data used is synthetic and created solely for learning, analysis, and portfolio demonstration purposes.

---

**Dashboard and Documentation by SOHAM S. AMBURLE**
**15 March 2026**
