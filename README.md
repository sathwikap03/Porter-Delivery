# Porter-Delivery
# Delivery Performance & Partner Efficiency Analysis

## Overview
This project focuses on analyzing **delivery performance data** to understand how factors such as **market**, **partner availability**, and **store category** influence **delivery times** and **operational efficiency**.  
The goal is to generate **data-driven insights** that help optimize delivery speed, resource allocation, and partner utilization.

The analysis was performed entirely in **Microsoft Excel**, using **formulas**, **PivotTables**, **charts**, and **interactive dashboards** with slicers and timelines.

## Dataset
**File:** Delivery_Performance_Dashboard.xlsx  
**Source:** Simulated delivery operations dataset  

### Description:
The dataset includes order and delivery information such as:
- Market ID and Store Details  
- Store Category (American, Mexican, etc.)  
- Delivery Protocol  
- Order Subtotal and Total Items  
- Partner Availability (On-shift, Busy, Outstanding)  
- Delivery and Order Creation Timestamps  

##  Tools & Techniques Used
- **Microsoft Excel**
  - Data Cleaning (Removing blanks, converting IDs, handling nulls)  
  - Calculated Columns for KPIs (Delivery Time, Partner Ratio, etc.)  
  - PivotTables & PivotCharts  
  - Conditional Formatting  
  - Interactive Slicers and Timeline Filters  
  - Dashboard Design (Layout, Colors, and KPIs)

##  Project Workflow

### 1️⃣ Data Cleaning & Preparation
- Converted market_id into numeric format  
- Replaced or removed null values in:
  - order_protocol
  - total_onshift_partners
  - total_busy_partners
  - total_outstanding_orders
- Created calculated columns:
  - **Delivery Time (mins)** → =(actual_delivery_time - created_at)*1440
  - **Partner Ratio** → =total_busy_partners/total_onshift_partners
  - **Hour of Order** → =HOUR(created_at)
  - **Day of Week** → =TEXT(created_at,"dddd")

## 📈 Dashboard Features

### 🔹 KPI Cards
- **Average Delivery Time (mins)**  
- **Total Orders**  
- **% of Orders Delivered <30 mins**  
- **Average Partner Ratio**  
- **Average Order Value**  

### 🔹 Visual Charts
- Market-wise Order Volume – Pie Chart
- Peak Order Hours – Line Chart 
- Top 5 Stores (Longest Delivery) – Horizontal Bar Chart
- Partner Availability vs Delivery Time – Scatter Plot
- Day of Week vs Avg Delivery Time – Column Chart 
- Store Category vs Average Delivery Time – Line Chart  

###  Interactive Filters
- Market  
- Store Primary Category  
- Order Protocol  
- Day of Week  

###  Timeline
- Based on 'created_at' to track delivery trends over time  

## 🧾 Key Insights
- Certain markets handle **higher order volumes**, indicating regional demand clusters.  
- **Store category** impacts delivery time — some cuisines take longer to deliver.    
- **Weekends** often experience **slower delivery times** due to higher traffic.  
- **Top 5 stores** with longest delivery times need operational review.  
- **Higher partner availability** leads to **faster deliveries**, confirming efficiency dependence.

##  How to Use
1. Open the Excel file.
2. Go to the **Dashboard** sheet.  
3. Use the **slicers** to filter by market, category, or order protocol.  
4. Use the **timeline** to view patterns over time.  
5. Review **KPI cards** for quick operational insights.  
6. Interact with charts to explore relationships between delivery time and partner metrics.

##  Future Improvements
- Integrate **Power Query** for automated data updates  
- Build a **Power BI version** for deeper insights and better visuals  
- Add predictive analytics for **estimated delivery time forecasting**  
- Include real-time order tracking integration for live monitoring  

##  Results Summary
The analysis provides actionable insights to:
- Improve **delivery speed** through better partner management  
- Identify **high-demand markets** for resource allocation  
- Highlight **store-level inefficiencies** for performance improvement  
- Support **data-driven decision-making** in delivery operations  

##  Author
**Pudota Sathwika**  
 **GitHub Profile:** [sathwikap03](https://github.com/sathwikap03)  
 **Email:** *[your email here]*  

