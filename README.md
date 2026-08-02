# 📱 Interactive Mobile Sales & Time-Intelligence Analytics Dashboard


<img width="750" height="450" alt="dashboard1" src="https://github.com/user-attachments/assets/0389e1f7-23e2-4b59-8324-f75501a823d8" />
<img width="750" height="450" alt="dashboard2" src="https://github.com/user-attachments/assets/9a2d60d6-90c2-4f1a-82fe-b08bff739775" />
<img width="750" height="450" alt="dashboard3" src="https://github.com/user-attachments/assets/7acc0267-72f0-4ee9-b841-5055470ca136" />


# 📱 Mobile Sales Analytics Dashboard
### *Driving Data-Driven Decisions for a Multi-Brand Retail Chain*

---

## 🚀 Project Overview
In the highly competitive mobile phone retail market, understanding sales patterns, customer preferences, and regional performance is critical. This project transforms **3,831 raw transactional records** (spanning **3+ years**) into an **interactive Power BI dashboard**.

The dashboard serves as a single source of truth for stakeholders, enabling them to monitor **$769M+ in sales**, analyze **brand performance**, optimize **inventory allocation**, and improve **customer satisfaction**—all in real-time.

---

## 🎯 The Business Problem
- **Challenge:** The retail chain lacked a unified view of sales performance across 30+ cities and 5 major brands (Apple, Samsung, OnePlus, Vivo, Xiaomi).
- **Goal:** Build a scalable analytics solution to track KPIs, identify growth opportunities, and understand customer buying behavior.
- **Outcome:** A dynamic dashboard that reduces reporting time by **90%** and provides actionable insights for the executive team.

---

## 📊 Key Performance Indicators (KPIs)

| Metric | Value | Insight |
| :--- | :--- | :--- |
| **Total Sales** | **$769M** | Strong revenue generation over the period. |
| **Total Quantity Sold** | **19K Units** | Average ticket size is high (~$40K per transaction). |
| **Total Transactions** | **4,000+** | Consistent daily sales volume. |
| **Average Order Value** | **$40K** | Indicates a premium customer segment. |
| **Time Period** | Oct 2021 – Oct 2024 | Captures post-COVID recovery and growth trends. |

---

## 🔍 Key Business Insights

### 1. Brand Performance & Market Share
- **Apple** leads with **$161.6M**, closely followed by **Samsung** ($160M).
- **OnePlus** ($153.7M), **Vivo** ($150M), and **Xiaomi** ($143M) form a strong mid-tier.
- *Actionable Takeaway:* Premium brands (Apple/Samsung) drive maximum revenue; consider exclusive promotions for mid-tier brands to boost their share.

### 2. Top-Selling Mobile Models
- **iPhone SE**, **OnePlus Nord**, and **Galaxy Note 20** are the top 3 best-sellers.
- *Actionable Takeaway:* These models should be prioritized in inventory and marketing campaigns.

### 3. Geographic Sales Distribution
- **Delhi** and **Mumbai** are the highest-performing cities, contributing a significant portion of total revenue.
- *Actionable Takeaway:* Allocate more marketing budget to these metropolitan hubs while strategizing penetration into emerging cities (e.g., Ludhiana, Gorakhpur).

### 4. Temporal Sales Trends
- **Year-over-Year (YoY):** Sales grew consistently from $58.8M (2021) to **$76.9M (2024)** , indicating a healthy 30%+ growth trajectory.
- **Monthly Seasonality:** **January** consistently shows the highest sales (0.2Bn), likely driven by New Year/ festive demand.
- *Actionable Takeaway:* Plan major promotional campaigns around January and Q4.

### 5. Customer Ratings & Experience
- Majority of customers rate products as **"Good"**, with only 27.6% rating as "Poor".
- *Actionable Takeaway:* Investigate the 27.6% poor rating cohort to identify specific model/city pain points.

### 6. Payment Method Analysis
- **UPI** and **Debit Card** are the most preferred payment methods.
- *Actionable Takeaway:* Ensure smooth UPI integration and offer cashback on digital payments to increase conversion.

---

## 🛠️ Technical Architecture & Skills Demonstrated

| Layer | Technology / Skill |
| :--- | :--- |
| **Data Preparation** | Power Query (Excel/CSV transformation, data cleaning, type casting). |
| **Data Modeling** | Star Schema design, Date Table creation for time intelligence. |
| **DAX (Calculations)** | Total Sales, Total Quantity, SPLY (Same Period Last Year), MTD (Month-to-Date), YoY Growth %. |
| **Visualization** | Power BI (Interactive slicers, line charts, bar charts, cards, matrices). |
| **Version Control** | Git & GitHub for project documentation. |

---

## 📁 Data Model & Structure

**Source:** `mobile_sales_data.xlsx` (3,831 rows, 14 columns)

**Key Dimensions:**
- **Date:** Day, Month, Year, Day Name (supports SPLY and MTD).
- **Product:** Brand, Mobile Model.
- **Customer:** Customer Name, Age, City.
- **Transaction:** Payment Method, Customer Ratings.

**Fact Table:**
- Units Sold, Price Per Unit (used to calculate Total Sales).

---

## 📸 Dashboard Previews

> *The dashboard provides three distinct views for granular analysis:*

1.  **Executive View:** High-level KPIs, brand performance, and city-wise sales.
2.  **Time-Series View:** YoY, MTD, and SPLY comparisons to track growth.
3.  **Product View:** Drill-down into specific models and ratings.

---
