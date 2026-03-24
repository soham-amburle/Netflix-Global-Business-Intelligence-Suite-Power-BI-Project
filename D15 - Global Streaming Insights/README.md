# Global Streaming Intelligence Suite – Global Streaming Insights

**Organization:** Netflix (Simulated Streaming Analytics Model)  
**Tool:** Power BI  
**Dataset:** Synthetic Global Streaming Dataset – ~2,394 Records  
**Dashboard Focus:** Executive Overview of Global Performance, Engagement, Revenue, and Content  
**Date:** 24 March 2026  
**Created by:** Soham S. Amburle  

---

## Overview

The **Global Streaming Insights Dashboard** serves as the executive summary of the entire streaming analytics suite, bringing together key metrics across users, content, revenue, engagement, and churn.

Built using a synthetic dataset and a snowflake schema data model, this dashboard provides leadership with a **holistic view of platform performance across global markets**.

This dashboard answers strategic business questions:

* What is the overall scale of the platform in terms of users and content?
* How engaged are users across the platform?
* How is revenue distributed across subscription plans?
* What content types dominate the platform?
* How does performance vary across global regions?

Through KPI cards, maps, and summary visuals, this dashboard delivers a **high-level, decision-focused overview of streaming performance**.

---

## Business Storyline & Analytical Flow

### 1. Executive KPI Snapshot

Eight KPI cards provide a unified performance overview:

* **Total Users**
* **Total Watch Hours**
* **Total Revenue**
* **Total Content**
* **Avg Rating**
* **Total Streams**
* **Churn Rate (%)**
* **ARPU**

These KPIs allow leadership to quickly assess **growth, engagement, monetization, and retention health**.

---

### 2. Main Analytical Visuals

Four visuals summarize key business dimensions:

1. **GLOBAL STREAMING MAP** – Map (Unit: Watch Hours)  
2. **WATCH HOURS BY GENRE** – Bar Chart (Unit: Watch Hours)  
3. **REVENUE BY PLAN** – Column Chart (Unit: Revenue)  
4. **CONTENT TYPE DISTRIBUTION** – Donut Chart (Unit: %)  

These visuals provide insights into **geographic performance, content consumption, revenue streams, and catalog composition**.

---

### 3. Interactive Slicers

Eight slicers enable cross-dimensional exploration:

* Continent (`Dim_Geography[Continent]`)
* Country (`Dim_Geography[Country]`)
* Content Type (`Dim_Content[ContentType]`)
* Genre (`Dim_Genre[GenreName]`)
* Language (`Dim_Language[LanguageName]`)
* Subscription Plan (`Dim_SubscriptionPlan[PlanName]`)
* Gender (`Dim_Users[Gender]`)
* Age Group (`Dim_Users[Age Group]`)

These slicers allow stakeholders to analyze performance across **geography, content, and user segments**.

---

## Key Takeaways

This dashboard enables stakeholders to:

* Monitor overall platform performance in one unified view  
* Evaluate engagement through watch hours and streams  
* Understand revenue contribution across subscription plans  
* Analyze content consumption trends across genres  
* Compare performance across global regions  
* Support executive decision-making with high-level insights  

---

## Tools & Data

* **Visualization Tool:** Power BI  
* **Dataset:** Synthetic global streaming dataset  
* **Record Count:** ~2,394 rows  
* **Data Model:** Snowflake Schema  
* **Purpose:** Executive-level streaming analytics overview  

---

> **Note:** This project is not affiliated with Netflix. All data is synthetic and created solely for educational and portfolio purposes.

---

**Dashboard and Documentation by SOHAM S. AMBURLE**  
**24 March 2026**
