# Global Streaming Intelligence Suite – Watch Behaviour Analysis

**Organization:** Netflix (Simulated Streaming Analytics Model)
**Tool:** Power BI
**Dataset:** Synthetic Global Streaming Dataset – ~2,394 Records
**Dashboard Focus:** User Viewing Behavior, Engagement Patterns, and Streaming Trends
**Date:** 16 March 2026
**Created by:** Soham S. Amburle

---

## Overview

The **Watch Behaviour Analysis Dashboard** provides a comprehensive view of how users interact with content on a global streaming platform inspired by Netflix. Built using a synthetic dataset, this dashboard focuses on analyzing **watch time, session behavior, content consumption patterns, and device usage trends**.

This dashboard enables stakeholders to understand **how users engage with content**, identify viewing patterns, and evaluate platform engagement across different dimensions such as content type, genre, geography, and device usage.

It answers key analytical questions such as:

* How much time are users spending on the platform?
* What is the average watch duration per session?
* What percentage of content is fully completed?
* Which devices are most commonly used for streaming?
* How does watch behavior vary across genres and content types?

Through KPI cards, interactive slicers, and visual charts, this dashboard delivers an **insightful view into user engagement and streaming behavior**.

---

## Business Storyline & Analytical Flow

### 1. KPI Snapshot – User Engagement Overview

Six KPI cards provide an immediate overview of viewing behavior:

* **Total Watch Hours**
* **Total Watch Sessions**
* **Average Watch Time**
* **Completion Rate (%)**
* **Average Sessions per User**
* **Average Watch Hours per User**

These KPIs help stakeholders quickly assess **platform engagement and user activity levels**.

---

### 2. Main Visualizations – Viewing Behavior Insights

The dashboard includes five key visuals:

1. **WATCH TIME DISTRIBUTION BY CONTENT TYPE** – Clustered Column Chart
2. **WATCH TIME BY DEVICE TYPE** – Donut Chart
3. **AVERAGE WATCH TIME BY GENRE** – Bar Chart
4. **WATCH SESSIONS BY USER (ENGAGEMENT DISTRIBUTION)** – Column Chart
5. **WATCH HOURS BY COUNTRY** – Map Visualization

These visuals provide a **multi-dimensional view of user behavior**, covering content preferences, device usage, and geographic engagement.

---

### 3. Interactive Slicers

Six slicers enable dynamic filtering of the dashboard:

* Continent (`Dim_Geography[Continent]`)
* Country (`Dim_Geography[Country]`)
* Content Type (`Dim_Content[ContentType]`)
* Genre (`Dim_Genre[GenreName]`)
* Device Type (`Dim_Device[DeviceType]`)

These filters allow users to explore **watch behavior across different segments and regions**.

---

## Key Takeaways

This dashboard enables analysts and stakeholders to:

* Understand overall user engagement and viewing intensity
* Analyze how content type and genre influence watch time
* Evaluate device preferences for streaming
* Identify high-engagement regions and countries
* Monitor completion rates to assess content effectiveness

---

## Tools & Data

* **Visualization Tool:** Power BI
* **Dataset:** Synthetic global streaming dataset
* **Total Records:** ~2,394 rows
* **Data Model:** Snowflake Schema
* **Fact Tables:** Watch History, Subscriptions, Ratings
* **Dimension Tables:** Users, Content, Genre, Language, Geography, Device, Subscription Plan, Time
* **Data Generation Tool:** Mockaroo

---

> **Note:** This project is not affiliated with Netflix. All data used in this dashboard is synthetic and created solely for learning, analysis, and portfolio demonstration purposes.

---

**Dashboard and Documentation by SOHAM S. AMBURLE**
**16 March 2026**
