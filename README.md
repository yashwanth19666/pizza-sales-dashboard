# pizza-sales-dashboard# 🍕 Pizza Sales Dashboard – Tableau Business Analyst Project

## 📊 Project Overview
This project explores pizza sales data from **Plato's Pizza**, a Greek-inspired pizzeria in New Jersey. As a Business Intelligence Consultant, your goal is to use **Tableau** to uncover insights and improve restaurant operations.

---

## 🎯 Objectives
- Identify sales trends and patterns over time
- Analyze pizza performance (best/worst-sellers)
- Understand customer demand by day and time
- Calculate key business metrics like average order value
- Offer data-driven recommendations to boost efficiency and sales

---

## 🧰 Tools & Technologies
- **Tableau Desktop** – for dashboard creation and data visualization  
- **Excel** – for initial data review and cleaning  
- **SQL (optional)** – for data manipulation (if needed)

---

## 📁 Dataset Details

### Source
- [Maven Pizza Challenge Dataset](https://www.mavenanalytics.io/blog/maven-pizza-challenge)

### Main File
- `pizza_sales.csv`

### Features
- `order_id` – Unique order identifier  
- `order_date`, `order_time` – Timestamp of each order  
- `pizza_name`, `pizza_type`, `pizza_size`, `pizza_ingredients` – Product details  
- `quantity`, `unit_price`, `total_price` – Transactional data  
- 12 columns in total describing sales activity at Plato’s Pizza

---

## 📈 Key Business Questions
1. What days and times are busiest?
2. How many pizzas are made during peak periods?
3. What are the best and worst-selling pizzas?
4. What is the average order value?
5. How well is seating capacity (15 tables / 60 seats) utilized?

---

## 📌 Dashboard Design Steps

### 1. **Data Cleaning & Preparation**
- Remove inconsistencies and ensure correct data types
- Extract `Day of Week` and `Hour` from `order_date` and `order_time`
- Check for missing or duplicate values

### 2. **Load Data into Tableau**
- Connect to the CSV file in Tableau
- Perform field formatting (e.g., date/time)

### 3. **Create Visualizations**
- **Total Revenue Over Time** (Line Chart)
- **Revenue by Pizza Name** (Bar Chart)
- **Sales by Day of Week** (Bar Chart)
- **Sales by Time of Day** (Line Chart)
- **Average Order Value** (KPI Card)
- **Total Pizzas Sold** (KPI Card)

### 4. **Dashboard Assembly**
- Combine all key visuals into a single, interactive dashboard
- Add slicers/filters (e.g., pizza type, size)
- Use tooltips, annotations, and titles for clarity

---

## 📌 Example Calculated Fields in Tableau

```sql
// Day of Week
DATEPART('weekday', [order_date])

// Hour of Day
DATEPART('hour', [order_time])
