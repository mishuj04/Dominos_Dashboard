# 🍕 Domino's Pizza Sales Analysis Dashboard

## 📖 Project Overview
This project analyzes Domino’s Pizza sales data to uncover trends in customer behavior, revenue patterns, and product performance.  
The analysis pipeline involves **data preprocessing in Python (pandas)** and **interactive visualization in Power BI**.

The final Power BI dashboard delivers insights into **sales performance, product mix, order timing, and customer demand patterns**.

---

## 🧩 Dataset Description
The dataset contains detailed order-level data with the following key columns:

| Column Name | Description |
|--------------|-------------|
| `order_id` | Unique order identifier |
| `pizza_id` | Unique pizza item identifier |
| `pizza_name_id` | Pizza type and size ID |
| `pizza_name` | Full pizza name |
| `pizza_category` | Category (e.g., Classic, Supreme, Veggie, Chicken) |
| `pizza_size` | Size of pizza (S, M, L, XL, XXL) |
| `pizza_ingredients` | List of ingredients used |
| `quantity` | Quantity of each pizza ordered |
| `unit_price` | Price per unit |
| `total_price` | Total amount for each line item |
| `order_date` | Date of order |
| `order_time` | Time when the order was placed |

---

## 🧮 Data Preprocessing (in Python)
The raw dataset was cleaned and enriched using **pandas** before importing into Power BI.  
The following transformations were applied:

- Converted `order_time` to datetime format and extracted the `order_hour`.
- Created a new column `meal_time` based on the time of day (Breakfast, Lunch, Dinner, Late Night).
- Converted `order_date` to datetime type.
- Extracted `weekday_number` (0 = Monday, 6 = Sunday).
- Added a `weekend` flag (1 = Saturday/Sunday, 0 = Weekday).
- Calculated `ingredient_count` to measure pizza complexity based on ingredient list length.

These enriched features were used to generate time-based and behavioral insights in Power BI.

---

## 📊 Power BI Dashboard

### Dashboard Highlights
The interactive dashboard consists of multiple visual components providing a comprehensive business overview.

#### 🔹 **Top KPIs**
| KPI | Description |
|------|--------------|
| **AOV (Average Order Value)** | Average revenue per order |
| **Average Pizza Price** | Mean price of pizzas sold |
| **Total Orders** | Number of unique orders |
| **Total Revenue** | Total revenue generated |

#### 🔹 **Visualizations**
| Chart Title | Purpose |
|--------------|----------|
| **Total Revenue by Pizza Category** | Identifies top-performing categories (Classic, Supreme, Veggie, Chicken) |
| **Total Orders by Pizza Size** | Shows customer preference by size (L, M, S, etc.) |
| **Total Orders by Meal Time** | Displays demand patterns across Breakfast, Lunch, Dinner, and Late Night |
| **Total Orders by Weekday Number** | Highlights weekday vs. weekend order trends |
| **Weekend Slicer** | Enables focused filtering on weekend vs. weekday data |
| **Category and Weekday Filters** | Allow dynamic exploration by pizza category and day |

---

## 📈 Key Insights

### 🧾 Sales Summary
- **Total Revenue:** ~$817.9K  
- **Total Orders:** ~21K  
- **Average Order Value (AOV):** $38.31  
- **Average Pizza Price:** $16.49  

### 🍕 Category Performance
- **Classic pizzas** generate the highest revenue (~220K).  
- **Supreme** and **Veggie** follow closely, while **Chicken** slightly trails.  
- Indicates strong customer loyalty to traditional pizza types.

### 📏 Size Preferences
- **Large (L)** pizzas dominate with ~36% of total orders.  
- **Medium (M)** and **Small (S)** sizes contribute nearly equally (~32% each).  
- Minimal demand for XL and XXL pizzas.

### 🕒 Order Timing
- **Dinner** and **Lunch** are peak ordering times.  
- **Late-night** orders are low, suggesting limited late-hour operations.

### 📅 Weekday Patterns
- Demand peaks on **Fridays (weekday 4)**, showing strong end-of-week sales.  
- Slight dip over weekends, indicating weekday promotions are effective.

---

## 💡 Business Recommendations
1. **Promote combo deals** during Lunch and Dinner to increase order size and AOV.  
2. **Upsell larger sizes** through targeted offers to boost revenue.  
3. **Introduce weekend promotions** to balance weekday-weekend order volumes.  
4. **Enhance marketing for Classic pizzas** while experimenting with new Veggie options.  
5. **Optimize staffing** during peak hours (Lunch & Dinner).

---

## ⚙️ Tools & Technologies
- **Python** (pandas, datetime) – Data cleaning and feature engineering  
- **Power BI** – Visualization, KPI design, and dashboard development  
- **GitHub** – Version control and project documentation  
