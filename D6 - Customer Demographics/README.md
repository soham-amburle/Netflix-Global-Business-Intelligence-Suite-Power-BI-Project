# Global Streaming Subscriber Overview

**Organization:** Netflix (Simulated Global Streaming Platform)  
**Tool:** Power BI  
**Dataset:** Synthetic Streaming Dataset – 2,394 Records  
**Dashboard Focus:** Global Subscriber Distribution and Growth Analysis  
**Date:** 15 March 2026  
**Created by:** Soham S. Amburle  

---

## Overview

The **Global Subscriber Overview Dashboard** provides a comprehensive view of subscriber distribution across a simulated global streaming platform inspired by Netflix. Built using a synthetic dataset of 2,394 records, this dashboard enables stakeholders to analyze **subscriber distribution across continents, regions, and countries, along with growth trends and demographic segmentation**.

This dashboard serves as a foundational layer for understanding **global audience reach, market penetration, and subscriber concentration**, helping decision-makers identify high-growth markets and regional performance patterns.

This dashboard answers key business questions:

- How are subscribers distributed globally across continents and countries?  
- Which regions contribute the highest number of subscribers?  
- How is subscriber growth trending over time?  
- What is the demographic composition of subscribers globally?  
- Which markets show the highest adoption potential?  

---

## Business Storyline & Analytical Flow

### 1. Subscriber KPI Snapshot – KPI Cards

Six KPI cards provide a high-level overview:

- **Total Subscribers**  
- **Active Subscribers**  
- **Cancelled Subscribers**  
- **Subscriber Growth (YTD)**  
- **Average Subscriber Age**  
- **Subscribers per Region (Avg)**  

These KPIs provide a **quick snapshot of global subscriber scale and health**.

---

### 2. Global Distribution Visuals

The dashboard includes key visuals to analyze geographic distribution:

1. **SUBSCRIBERS BY COUNTRY** – Map Visualization  
2. **SUBSCRIBERS BY CONTINENT** – Clustered Bar Chart  
3. **SUBSCRIBERS BY REGION** – Column Chart  

These visuals help identify **high-performing markets and global distribution patterns**.

---

### 3. Growth Trend Analysis

- **SUBSCRIBER GROWTH OVER TIME** – Area Chart  

This visual highlights **how the subscriber base evolves over time**, enabling trend analysis and growth monitoring.

---

### 4. Demographic Insights

- **SUBSCRIBERS BY AGE GROUP** – Column Chart  
- **SUBSCRIBERS BY GENDER** – Donut Chart  

These visuals provide insight into **who the subscribers are**.

---

### 5. Interactive Slicers

Eight slicers enable flexible filtering:

- Continent (`Dim_Geography[Continent]`)  
- Region (`Dim_Geography[Region]`)  
- Country (`Dim_Geography[Country]`)  
- Year (`Dim_Time[Year]`)  
- Month (`Dim_Time[Month]`)  
- Gender (`Dim_Users[Gender]`)  
- Age (`Dim_Users[Age]`)  
- Subscription Plan (`Dim_SubscriptionPlan[PlanName]`)  

---

## Key Takeaways

This dashboard allows stakeholders to:

- Analyze global subscriber distribution across multiple geographic levels  
- Identify high-performing regions and countries  
- Track subscriber growth trends over time  
- Understand demographic composition of users  
- Support global expansion and market targeting strategies  

---

## Tools & Data

- **Visualization Tool:** Power BI  
- **Dataset:** Synthetic streaming analytics dataset  
- **Record Count:** ~2,394 rows  
- **Data Model:** Snowflake Schema  
- **Fact Tables:** WatchHistory, Subscriptions, Ratings  
- **Dimension Tables:** Users, Content, Time, Geography, Genre, Language, Device, Subscription Plan  

---

> **Note:** This project is not affiliated with Netflix. All data is synthetic and created solely for portfolio and learning purposes.

---

**Dashboard and Documentation by SOHAM S. AMBURLE**  
**15 March 2026**
