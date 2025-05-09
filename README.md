# SQL-Sales-Performance-Analysis
Sales Performance Analysis of Walmart Stores Using Advanced MySQL Techniques

# 🛒 Walmart Sales Performance Analysis Using Advanced MySQL Techniques

## 📌 Project Overview

This project analyzes sales data from Walmart using **advanced SQL techniques** to uncover key insights related to branch performance, customer segmentation, product profitability, payment preferences, and shopping trends. The goal is to drive data-driven decisions for operational optimization.

## 🎯 Objective

To explore and analyze Walmart's transactional data using **MySQL** to:

- Identify top-performing branches
- Detect anomalies in sales transactions
- Segment customers by spending behavior
- Determine the most profitable product lines
- Discover preferred payment methods
- Understand trends in sales by gender and day of the week

## 🗃️ Dataset Overview

- **1000** sales transactions
- **15** unique customers
- **3** branches (A, B, C)
- **6** product lines
- Time period: **3 months** in **2019**

---

## 🧩 Key Analytical Tasks

### 1. 📈 Top Branch by Sales Growth Rate
- Calculated monthly sales per branch
- Used window functions (`LAG`) to compute monthly growth rates
- Found **Branch A** had the highest **average growth rate**, while **Branch C** had the **highest total sales**

### 2. 💰 Most Profitable Product Line per Branch
- Calculated profit as `gross_income - cogs`
- Used ranking techniques (e.g., `DENSE_RANK`, subqueries, and CTEs) to identify:
  - **Health and Beauty** (Branch A)
  - **Food and Beverages** (Branch B)
  - **Home and Lifestyle** (Branch C)

### 3. 🧍 Customer Segmentation by Spending
- Segmented customers into **Low**, **Medium**, and **High** spenders
- Used `SUM(cogs)` and `AVG(cogs)` for segmentation thresholds

### 4. 🚩 Detecting Anomalies in Sales Transactions
- Used 2 standard deviations from mean total per product line to flag outliers
- Identified unusually high/low transactions

### 5. 💳 Popular Payment Methods by City
- Used ranking logic to find most used payment method per city:
  - **Ewallet**: Popular in **Mandalay** and **Yangon**
  - **Cash**: More used in **Naypyitaw**

### 6. 👨‍👩‍👧 Monthly Sales by Gender
- Analyzed gender-based monthly sales trends
- Found **female customers** spent slightly more overall, especially in January

### 7. 🛍️ Best Product Line by Customer Type
- Identified top product lines preferred by **Members** and **Normal** customers

### 8. 🔁 Identifying Repeat Customers
- Used window functions and `DATEDIFF()` logic to identify customers who shopped multiple times within 30 days

### 9. 🥇 Top 5 Customers by Sales Volume
- Ranked and limited results to show top 5 revenue-generating customers

### 10. 📅 Sales Trends by Day of the Week
- Used `DAYNAME()` to extract sales distribution by weekdays
- Identified high-performing days for optimized inventory planning

---

## 📊 Key Insights

- **Branch A** showed the highest **average monthly growth**
- **Health and Beauty**, **Food & Beverages**, and **Home & Lifestyle** were top profitable lines across branches
- Most customers fall in the **Medium spending** category; High and Low are nearly equal
- **Ewallet** is the preferred payment method in most cities
- **January** had the highest overall sales; females generally spent more than males
- Sales showed **day-wise variations**—valuable for staffing and stock planning

---

## 💡 Recommendations

- 🚀 **Boost High-Growth Branches**: Invest in customer incentives and predictive inventory planning
- 🧴 **Expand High-Performing Product Lines**: Increase stock and promotions on top items
- 🎯 **Customer Retention Strategy**: Introduce loyalty programs for high spenders and offer targeted deals to medium/low spenders
- 💳 **Optimize Payment Channels**: Promote preferred payment methods using cashback or rewards

---

## 📽️ Project Presentation Video

▶️ [Watch the full walkthrough](https://drive.google.com/file/d/1dd52NZPHI8rhRcmKX2emzJqhaPemAlmf/view?usp=sharing)

---

👤 *Created by Ruturaj T. Saravane*
