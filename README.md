# 📱 Interactive Mobile Sales & Time-Intelligence Analytics Dashboard


<img width="750" height="450" alt="dashboard1" src="https://github.com/user-attachments/assets/0389e1f7-23e2-4b59-8324-f75501a823d8" />
<img width="750" height="450" alt="dashboard2" src="https://github.com/user-attachments/assets/9a2d60d6-90c2-4f1a-82fe-b08bff739775" />
<img width="750" height="450" alt="dashboard3" src="https://github.com/user-attachments/assets/7acc0267-72f0-4ee9-b841-5055470ca136" />



An end-to-end interactive Power BI analytical project engineered to track mobile sales performance, time-intelligence parameters (YoY / MTD growth), customer payment preferences, brand market share, and regional revenue distribution.

---

## 📸 Dashboard Screenshots

| Main Dashboard | MTD Performance Report | YoY / Same Period Last Year |
| :---: | :---: | :---: |
| ![Dashboard Overview](dashboard1.png) | ![MTD Report](dashboard2.png) | ![SPLY Analysis](dashboard3.png) |

---

## 📌 Executive Summary & Key KPIs

* **Total Revenue Generated:** ₹769.2M
* **Total Units Sold:** 19.15K units
* **Total Transactions:** 3,835 transactions
* **Average Transaction Value:** ₹40K
* **Top Revenue Brand:** Apple (₹161.6M) followed closely by Samsung (₹160.0M)
* **Top Handset Models:** iPhone SE (₹59.5M), OnePlus Nord (₹57.8M), Galaxy Note 20 (₹56.0M)

---

## 📊 Business Features & Dashboard Pages

### 1. Main Overview Dashboard Page
* **Geographical Distribution:** Real-time spatial tracking across Tier-1 and Tier-2 Indian cities (Mumbai, Delhi, Bangalore, Hyderabad, Patna, Ranchi, Gorakhpur, etc.) using spatial mapping.
* **Brand & Model Analysis:** Drill-down reporting to identify revenue drivers and fast-moving SKUs.
* **Payment Preference Mix:** Distribution analysis tracking cash vs digital modes (UPI, Credit Card, Debit Card).
* **Day-of-Week Revenue Velocity:** Visual tracking of daily revenue spikes showing elevated customer transactions during weekends (Saturday & Sunday).
* **Customer Feedback Profiling:** Breakdown of sales based on customer ratings (*Good*, *Average*, *Poor*).

### 2. MTD (Month-To-Date) Report
* **Cumulative Sales Trajectory:** Line graph representation tracking daily revenue progression within any selected month and year.
* **Run-Rate & Pacing Analysis:** Enables business leads to compare mid-month targets against actual cumulative sales trajectories (e.g., February 2023 achieving ₹19M across 95 transactions).

### 3. YoY Performance & Time Intelligence
* **Comparative Matrix:** Measures active performance against historical baselines (**Same Period Last Year - SPLY**) across years, quarters, and months.
* **Quarterly & Monthly Performance Trends:** Highlights cyclical spikes and dips to improve inventory allocation before peak quarters.

---

## 🛠️ Data Modeling & Advanced DAX Calculations

A custom **Date Table** was modeled in Power Query and connected via a 1-to-many relationship with the main sales dataset to enable robust Time Intelligence calculations.

### Core DAX Measures Used:

```dax
// Total Revenue Measure
Total Sales = SUM('Mobile Sales'[Sales Amount])

// Total Quantity Sold
Total Quantity = SUM('Mobile Sales'[Units Sold])

// Total Transaction Count
Transactions = COUNTROWS('Mobile Sales')

// Average Transaction Value
Average = DIVIDE([Total Sales], [Transactions], 0)

// Time Intelligence: Same Period Last Year (SPLY)
Same Period Last Year = 
CALCULATE(
    [Total Sales], 
    SAMEPERIODLASTYEAR('Calendar'[Date])
)

// Time Intelligence: Month-To-Date Sales
MTD Sales = 
TOTALMTD(
    [Total Sales], 
    'Calendar'[Date]
)
