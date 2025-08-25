# 🚖 Uber Trip Analysis Dashboard - README

## 📌 Project Overview
This project is a **Power BI Dashboard** built to analyze **Uber Trip Data** for June 2024. The dashboard provides insights into trip bookings, revenue, distance, passenger behavior, payment methods, and time-based trends. It is designed for business users, data analysts, and operations teams to track Uber's performance across different locations, vehicles, and payment methods.

---

## 📂 Data Model
The dashboard is powered by a **star schema model** with the following tables:

### 📊 Trip Details (Fact Table)
- DOLocationID
- Drop Off Time
- fare_amount
- passenger_count
- Payment_type
- Pickup date
- Pickup Hour (HH MM SS)
- Pickup Time
- Pickup Hour (derived)

### 🏙️ Location Table (Dimension Table)
- LocationID
- Location
- City

### 📅 Calendar Table (Dimension Table)
- Date
- Day_name
- Day_number

### ⚡ DAX Measures Table (Calculated KPIs)
- Avg Booking Value
- Avg Trip Distance (Miles)
- Avg Trip Time (Minutes)
- Total Booking Value

### 🔄 Dynamic Measure Table (for flexible KPI selection)
- Dynamic Measure
- Dynamic Measure Fields
- Dynamic Measure Order

---

## 📊 Dashboard Pages
The dashboard is divided into **three main sections** for easy navigation:

### 1️⃣ Overview Page
- **KPIs:**
  - 🚗 Total Bookings (103.7K)
  - 💵 Total Booking Value ($1.6M)
  - 📉 Avg Booking Value ($15)
  - 📍 Total Trip Distance Miles (348.9K)
  - 📏 Avg Trip Distance Miles (3.36)
  - ⏱ Avg Trip Time Minutes (16)

- **Visuals:**
  - 🍩 Donut Charts → Trip distance by **Payment Type** and **Day/Night**
  - 📈 Line Chart → Bookings by **Day**
  - 📊 Bar Charts → Bookings by **Vehicle Type** and **Location**
  - 🚙 Vehicle Analysis Table → Bookings, revenue, and trip distance per vehicle type

### 2️⃣ Time Analysis Page
- **KPIs:** (same as Overview for consistency)
- **Visuals:**
  - ⏰ Area Chart → Bookings by **Pickup Hour**
  - 🔲 Heatmap → Hourly bookings across weekdays
  - 📆 Line Chart → Bookings by **Day of the Week**

### 3️⃣ Details Page
- **Filters available:**
  - 📅 Date Range
  - 🏙️ City
  - 🚙 Vehicle Type
  - 💳 Payment Type
- **Detailed Trip Table:**
  - Trip ID, Pickup Date, Vehicle, Payment Type, No. of Passengers, Trip Distance, Booking Value, City, Pickup Location, Total Bookings

---

## 📈 Key Insights
1. 🚙 **Vehicle Preference:** UberX dominates with the highest share.
2. 💳 **Payment Trends:** Majority of payments are made using Uber Pay.
3. ⏰ **Time Trends:**
   - Bookings peak between **9 AM – 9 PM**.
   - Sundays and Saturdays record the **highest bookings**.
4. 📍 **Location Insights:** Top hotspots include Penn Station, Upper East Side, and Midtown.

---

## ⚙️ Features
- 🎚 **Interactive Slicers:** Date, City, Vehicle, Payment Type
- 🔄 **Dynamic Measures:** Switch between KPIs (Bookings, Revenue, Distance)
- 🔎 **Drill-through Capability:** From overview to trip-level details
- 📊 **Performance KPIs:** Highlighted at the top for clarity

---

## 🛠️ Tools & Technologies Used
- **Power BI Desktop** (dashboard creation)
- **DAX (Data Analysis Expressions)** (for calculated measures)
- **Data Modeling (Star Schema)**
- **Uber Trip Dataset (June 2024)**

---

## 🚀 How to Use
1. Open the Power BI dashboard.
2. Use **slicers (Date, City, Vehicle, Payment Type)** to filter data.
3. Navigate using the left-side menu:
   - 📊 **Overview:** High-level KPIs & summaries
   - ⏱ **Time Analysis:** Hourly & daily booking patterns
   - 📋 **Details:** Trip-level breakdown
4. Hover over visuals for **tooltips** with extra insights.

---

## 📌 Conclusion
This dashboard delivers a **360-degree analysis of Uber trips**, offering insights for:
- 🚗 **Operations Team** → Manage fleet & demand by location/time
- 💵 **Finance Team** → Track revenue & booking value
- 📊 **Business Analysts** → Understand customer behavior & optimize services

---

## 🖼️ Dashboard Snapshots

### 📊 Overview Page
![Overview Page](overview.png)

### ⏱ Time Analysis Page
![Time Analysis Page](time_analysis.png)

### 📋 Details Page
![Details Page](details.png)

---

📧 For queries or collaboration, please contact: *[Your Name / Team]*

