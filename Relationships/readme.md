# Data Modelling – Snowflake Schema Implementation

## Overview

This project follows a **Snowflake Schema data modelling approach**, which is widely used in enterprise-level streaming analytics platforms.

Instead of a flat transactional table, the dataset was structured into:

- Multiple **Fact tables** capturing user actions
- Multiple interconnected **Dimension tables**
- One-to-many relationships
- Single-direction filtering (Dimension → Fact)

This mirrors real-world BI architecture used by global streaming platforms such as Netflix.

---

## Step 1 – Fact Tables

Three fact tables were created to capture key platform events:

### 1. Fact_WatchHistory

Tracks all streaming sessions.

#### Keys
- WatchID (Primary Key)
- UserID (Foreign Key)
- ContentID (Foreign Key)
- DeviceID (Foreign Key)
- GeographyID (Foreign Key)
- DateID (Foreign Key)

#### Numeric / Transaction Attributes
- WatchMinutes
- CompletionFlag
- SessionID

---

### 2. Fact_Subscriptions

Captures subscription lifecycle.

#### Keys
- SubscriptionID (Primary Key)
- UserID (Foreign Key)
- PlanID (Foreign Key)
- GeographyID (Foreign Key)
- StartDateID (Foreign Key)
- EndDateID (Foreign Key)

#### Numeric / Transaction Attributes
- MonthlyPrice
- Status (Active / Cancelled)

---

### 3. Fact_Ratings

Tracks user ratings for content.

#### Keys
- RatingID (Primary Key)
- UserID (Foreign Key)
- ContentID (Foreign Key)
- DateID (Foreign Key)

#### Numeric / Transaction Attributes
- RatingScore (1–5)

---

## Step 2 – Dimension Tables

### Dim_Users

Columns:
- UserID (Primary Key)
- FirstName
- LastName
- Gender
- Age
- CountryID (Foreign Key)
- SignupDateID (Foreign Key)
- Email

---

### Dim_Content

Columns:
- ContentID (Primary Key)
- Title
- ContentType (Movie / Series)
- GenreID (Foreign Key)
- LanguageID (Foreign Key)
- ReleaseYear
- DurationMinutes
- ProductionCountryID (Foreign Key)

---

### Dim_Genre

Columns:
- GenreID (Primary Key)
- GenreName (e.g., Drama, Action, Comedy…)

---

### Dim_Language

Columns:
- LanguageID (Primary Key)
- LanguageName (e.g., English, Spanish…)

---

### Dim_Geography

Columns:
- GeographyID (Primary Key)
- Country
- Region
- Continent

---

### Dim_Device

Columns:
- DeviceID (Primary Key)
- DeviceType (Mobile, Smart TV, Desktop, Tablet, Console)

---

### Dim_SubscriptionPlan

Columns:
- PlanID (Primary Key)
- PlanName (Basic / Standard / Premium)
- MonthlyPrice
- MaxDevices

---

### Dim_Time

Columns:
- DateID (Primary Key)
- Date
- Year
- Month
- Quarter

> The Date Dimension enables time intelligence calculations such as YoY, MTD, and QTD.

---

## Step 3 – Relationship Configuration

### Fact → Dimension Relationships

**Fact_WatchHistory**
- `Dim_Users[UserID]` → `Fact_WatchHistory[UserID]`  
- `Dim_Content[ContentID]` → `Fact_WatchHistory[ContentID]`  
- `Dim_Device[DeviceID]` → `Fact_WatchHistory[DeviceID]`  
- `Dim_Geography[GeographyID]` → `Fact_WatchHistory[GeographyID]`  
- `Dim_Time[DateID]` → `Fact_WatchHistory[DateID]`  

**Fact_Subscriptions**
- `Dim_Users[UserID]` → `Fact_Subscriptions[UserID]`  
- `Dim_SubscriptionPlan[PlanID]` → `Fact_Subscriptions[PlanID]`  
- `Dim_Geography[GeographyID]` → `Fact_Subscriptions[GeographyID]`  
- `Dim_Time[StartDateID]` → `Fact_Subscriptions[StartDateID]`  

**Fact_Ratings**
- `Dim_Users[UserID]` → `Fact_Ratings[UserID]`  
- `Dim_Content[ContentID]` → `Fact_Ratings[ContentID]`  
- `Dim_Time[DateID]` → `Fact_Ratings[DateID]`  

### Dimension → Dimension Relationships

- `Dim_Content[GenreID]` → `Dim_Genre[GenreID]`  
- `Dim_Content[LanguageID]` → `Dim_Language[LanguageID]`  

---

### Relationship Settings

- **Cardinality:** Many-to-One (*:1)  
- **Cross-filter direction:** Single (Dimension → Fact)  
- **Active relationships:** Enabled  

---

## Final Data Model Structure

Dim_Users — Fact_WatchHistory — Dim_Time  
Dim_Content — Fact_WatchHistory — Dim_Device  
Dim_Content — Dim_Genre  
Dim_Content — Dim_Language  

Fact_Subscriptions → Dim_Users / Dim_SubscriptionPlan / Dim_Geography / Dim_Time  
Fact_Ratings → Dim_Users / Dim_Content / Dim_Time  

---

## Model Characteristics

- True **Snowflake Schema** with dimension normalization  
- No bidirectional filtering  
- Clean hierarchical structure for drill-downs  
- Optimized for **performance and scalability**  
- Supports **multi-level analytics**: Global → Continent → Country → Content → User behavior

---

## Why Snowflake Schema?

- Reduces data redundancy  
- Improves filter and slice performance  
- Reflects real-world streaming platform BI architecture  
- Facilitates advanced analytics across multiple dimensions  
