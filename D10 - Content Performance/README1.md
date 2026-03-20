# Global Streaming Intelligence Suite – Content Performance Analysis

**Organization:** Netflix (Simulated Streaming Analytics Model)  
**Tool:** Power BI  
**Dataset:** Synthetic Global Streaming Dataset – ~2,394 Records  
**Dashboard Focus:** Content Performance, Engagement, and Viewer Ratings Analysis  
**Date:** 19 March 2026  
**Created by:** Soham S. Amburle  

---

## Overview

The **Content Performance Dashboard** provides a comprehensive view of how content performs on a global streaming platform by analyzing **watch time, viewer engagement, and audience ratings**.

Built using a synthetic dataset and a snowflake schema data model, this dashboard enables analysts to evaluate **which titles, genres, and content types drive the highest engagement and satisfaction**.

This dashboard answers key analytical questions:

* Which content titles generate the highest watch time?
* How does engagement vary across genres and content types?
* What is the overall viewer rating across content?
* Which titles are most highly rated by users?
* How effectively is content consumed (completion rate)?

Through KPI cards, charts, and slicers, the dashboard delivers an **interactive and performance-focused view of streaming content**.

---

## Business Storyline & Analytical Flow

### 1. Content Performance Snapshot – KPI Cards

Seven KPI cards provide a high-level overview:

* **Total Watch Hours**
* **Total Streams**
* **Unique Viewers**
* **Average Watch Time**
* **Completion Rate (%)**
* **Average Rating**
* **Total Content Titles**

These KPIs allow stakeholders to quickly assess **content engagement, scale, and quality**.

---

### 2. Main Analytical Visuals

Four visuals provide deeper performance insights:

1. **TOP 10 CONTENT BY WATCH HOURS** – Bar Chart (Unit: Hours)  
2. **WATCH HOURS BY GENRE** – Column Chart (Unit: Hours)  
3. **WATCH HOURS BY CONTENT TYPE** – Donut Chart (Unit: Distribution %)  
4. **TOP 10 CONTENT BY AVG RATING** – Bar Chart (Unit: Rating Score)  

These visuals help identify **high-performing content, audience preferences, and quality perception**.

---

### 3. Interactive Slicers

Seven slicers enable dynamic filtering:

* Content Type (`Dim_Content[ContentType]`)
* Genre (`Dim_Genre[GenreName]`)
* Language (`Dim_Language[LanguageName]`)
* Release Year (`Dim_Content[ReleaseYear]`)
* Country (`Dim_Geography[Country]`)
* Date (`Dim_Time[Date]`)
* Device Type (`Dim_Device[DeviceType]`)

These slicers allow exploration across **content attributes, geography, time, and device usage**.

---

## Key Takeaways

This dashboard enables stakeholders to:

* Identify top-performing content based on watch time  
* Understand audience preferences across genres and formats  
* Evaluate content quality using viewer ratings  
* Analyze engagement trends across regions and devices  
* Support data-driven content acquisition and production decisions  

---

## Tools & Data

* **Visualization Tool:** Power BI  
* **Dataset:** Synthetic global streaming dataset  
* **Record Count:** ~2,394 rows  
* **Data Model:** Snowflake Schema  
* **Purpose:** Content performance analytics for BI portfolio  

---

> **Note:** This project is not affiliated with Netflix. All data is synthetic and created solely for educational and portfolio purposes.

---

**Dashboard and Documentation by SOHAM S. AMBURLE**  
**19 March 2026**
