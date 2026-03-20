# Global Streaming Intelligence Suite – Device Usage Analytics

**Organization:** Netflix (Simulated Streaming Analytics Model)
**Tool:** Power BI
**Dataset:** Synthetic Global Streaming Dataset – 2,394 Records
**Dashboard Focus:** Device Usage Behavior, Streaming Patterns, and Engagement Analysis
**Date:** 17 March 2026
**Created by:** Soham S. Amburle

---

## Overview

The **Device Usage Analytics Dashboard** provides a detailed view of how users interact with a global streaming platform across different devices such as mobile, smart TV, desktop, tablet, and gaming consoles.

Built using a synthetic dataset of 2,394 records and a snowflake schema data model, this dashboard enables analysts and decision-makers to understand **device preferences, streaming behavior, engagement levels, and completion trends**.

This dashboard answers key analytical questions:

* Which devices are most used for streaming?
* How is watch time distributed across devices?
* Which devices generate the highest engagement?
* How does completion behavior vary by device?
* How does device usage differ across regions?

Through KPI cards, charts, and slicers, the dashboard provides an **interactive and insightful view of device-level streaming behavior**.

---

## Business Storyline & Analytical Flow

### 1. Device KPI Snapshot – KPI Cards

Six KPI cards provide a quick overview of device usage:

* **Total Watch Hours**
* **Total Streams**
* **Unique Users**
* **Most Used Device**
* **Average Watch Time per Device**
* **Completion Rate**

These KPIs help stakeholders quickly assess **platform usage and engagement across devices**.

---

### 2. Main Analytical Visuals

Five key visuals provide device-level insights:

1. **DEVICE USAGE DISTRIBUTION** – Donut Chart (Unit: Streams %)
2. **WATCH HOURS BY DEVICE** – Clustered Bar Chart (Unit: Hours)
3. **DEVICE USAGE BY CONTINENT** – Stacked Column Chart (Unit: Streams)
4. **AVG WATCH TIME BY DEVICE** – Clustered Bar Chart (Unit: Minutes)
5. **COMPLETION RATE BY DEVICE** – Area Chart (Unit: %)

These visuals help identify **device preferences, engagement levels, and regional usage patterns**.

---

### 3. Interactive Slicers

Eight slicers allow dynamic filtering:

* Date (`Dim_Time[Date]`)
* Device Type (`Dim_Device[DeviceType]`)
* Continent (`Dim_Geography[Continent]`)
* Country (`Dim_Geography[Country]`)
* Content Type (`Dim_Content[ContentType]`)
* Genre (`Dim_Genre[GenreName]`)
* Subscription Plan (`Dim_SubscriptionPlan[PlanName]`)
* Language (`Dim_Language[LanguageName]`)

These slicers enable users to explore device usage across **geography, content, and user preferences**.

---

## Key Takeaways

This dashboard enables stakeholders to:

* Identify the most popular streaming devices
* Analyze watch time distribution across devices
* Understand user engagement patterns
* Compare completion rates across device types
* Explore regional differences in device usage

---

## Tools & Data

* **Visualization Tool:** Power BI
* **Dataset:** Synthetic global streaming dataset
* **Record Count:** ~2,394 rows
* **Data Model:** Snowflake Schema
* **Purpose:** Device usage analytics for streaming platform BI portfolio

---

> **Note:** This project is not affiliated with Netflix. All data used in this dashboard is synthetic and created solely for learning, analysis, and portfolio demonstration purposes.

---

**Dashboard and Documentation by SOHAM S. AMBURLE**
**17 March 2026**
