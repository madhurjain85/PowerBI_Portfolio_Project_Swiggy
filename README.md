# 🍔 Power BI Portfolio Project – Swiggy Food Delivery Analysis

## 📊 Project Overview
This project presents an **end-to-end Business Intelligence solution using Power BI** to analyze food delivery operations similar to **Swiggy in Bengaluru, India**.
The objective is to transform messy transactional data into a **clean, structured analytical model**, build **DAX-driven KPIs**, and create **interactive dashboards** that provide insights into:
* Revenue performance
* Delivery efficiency
* Customer behavior
* Restaurant ratings

The project demonstrates the complete **data analytics workflow** including **data cleaning, data modeling, KPI development, and dashboard design**.


# 🎯 Business Objectives
The project aims to simulate a real-world **Food Delivery Analytics System** by achieving the following goals:
* Clean and standardize raw delivery data
* Build a scalable **Star Schema data model**
* Create business KPIs using **DAX**
* Design interactive dashboards for business users
* Generate **actionable insights** for decision making

# 🗂 Dataset Overview
The dataset simulates **Swiggy food delivery orders across Bengaluru** and contains operational, transactional, and customer feedback data.

### Key Columns

| Column            | Description                      |
| ----------------- | -------------------------------- |
| `order_id`        | Unique order identifier          |
| `order_time`      | Order placement timestamp        |
| `delivery_time`   | Delivery completion time         |
| `restaurant_name` | Name of the restaurant           |
| `cuisine_type`    | Cuisine category                 |
| `location`        | Delivery area                    |
| `total_amount`    | Order value                      |
| `ordered_qty`     | Quantity ordered                 |
| `rating`          | Customer rating                  |
| `online_order`    | Online / Offline order indicator |
| `book_table`      | Table booking indicator          |
| `distance_km`     | Delivery distance                |


# 🧹 Data Cleaning (Power Query)
Data preprocessing was performed using **Power Query** to ensure high-quality analytical data.
Key cleaning steps:

* Handled missing values in **rating, online_order, and book_table**
* Standardized **city names and text formatting**
* Converted rating values such as **"4.5/5" → numeric**
* Applied business logic rules:

```
If online_order = 'No'
Then delivery_time = NULL
And distance_km = NULL
```

* Ensured correct data types for all columns

---

# 🏗 Data Modeling (Star Schema)

A **Star Schema model** was implemented for efficient reporting and analysis.
### Fact Table
**Fact_Orders**

| Column         |
| -------------- |
| order_id       |
| restaurant_key |
| location_key   |
| time_key       |
| total_amount   |
| ordered_qty    |
| distance_km    |
| rating_numeric |

---

### Dimension Tables

#### Dim_Restaurant
* restaurant_key
* restaurant_name
* cuisine_type

#### Dim_Location
* location_key
* area_name
* city_name

#### Dim_Time
* time_key
* timestamp
* hour
* day_name
* is_weekend
---

# 📈 Key Business Questions
The analysis focuses on solving real-world business problems.

---

## 💰 Sales & Revenue Analysis
1. What is the **total revenue generated across all orders?**
2. Which are the **top 5 cuisines by revenue?**
3. Which **location generates the highest sales?**
4. What is the **average order value (AOV)?**
5. What are the **top 10 high-value orders?**
---

## 🚚 Operational Efficiency
6. What is the **average delivery time for online orders?**
7. Which **restaurants deliver food the fastest?**
8. Which **location has the highest delivery delay?**
9. What is the **average delivery time for orders above 10 km?**
10. What is the **delivery success rate?**
---

## 👥 Customer Behavior
11. What percentage of orders are **online vs offline?**
12. Do customers who **book tables spend more?**
13. What are the **peak order hours?**
14. Which locations have the **highest order volume?**
15. What is the **average order quantity by cuisine?**
---

## ⭐ Quality & Ratings
16. Which restaurants have **average ratings above 4.5?**
17. Which cuisine has the **highest customer rating?**
18. Is there a **correlation between high spending and ratings?**
19. Which restaurants have **low ratings but high order volume?**
20. What is the **overall average rating across Bengaluru?**
---

# 📊 Power BI Dashboards
The Power BI report contains **three analytical dashboards**.

---

## 📌 Dashboard 1 – Sales Performance
Key metrics:
* Total Revenue
* Average Order Value
* Revenue by Cuisine
* Revenue by Location

Business insight:
Identifies **top-performing cuisines and high-revenue locations**.

---

## 🚚 Dashboard 2 – Delivery Operations

Key visuals:
* Average Delivery Time
* Delivery Distance vs Time
* Fastest Restaurants
* Delivery delays by location

Business insight:
Helps analyze **operational efficiency and delivery performance**.

---

## 👥 Dashboard 3 – Customer Insights

Key visuals:
* Online vs Offline Orders
* Peak Order Hours
* Top Rated Restaurants
* Order volume by location

Business insight:
Provides understanding of **customer ordering behavior**.

---

# 🧠 Key Skills Demonstrated

This project showcases practical skills used by **Data Analysts and BI Developers**.

* Power BI
* Power Query
* Data Cleaning
* Data Modeling (Star Schema)
* DAX Measures
* Business KPI Development
* Dashboard Design
* Data Visualization
* Business Insights

---

# 🚀 Business Impact

This project demonstrates how **data analytics can improve food delivery operations** by:

* Identifying high-revenue cuisines and restaurants
* Detecting delivery inefficiencies
* Understanding peak demand patterns
* Improving customer satisfaction through rating analysis

---

# 📬 Contact

If you found this project useful or want to collaborate:

**Madhur Jain**

* Data Analytics Consultant
* Microsoft Certified Trainer (MCT)
* Power BI | Microsoft Fabric | SQL | Azure

🔗 LinkedIn - www.linkedin.com/in/madhurjain85

---
