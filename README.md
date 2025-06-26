# 🛒 Zepto Data Analysis – SQL Project

This project is a SQL-based data exploration and analysis of Zepto-style e-commerce data. The goal is to clean, explore, and derive insights from a sample dataset that mimics real-world grocery delivery platform data.

---

## 📁 Files

- [`Zepto Data Analysis SQL Project.sql`](./Zepto%20Data%20Analysis%20SQL%20Project.sql):  
  Contains all SQL queries including table creation, data cleaning, and analysis.

---

## 🧹 Data Cleaning

- Dropped rows where MRP or discounted price is zero
- Converted prices from **paise to rupees**
- Handled missing (`NULL`) values
- Removed duplicate SKUs for same product names
- Identified and categorized out-of-stock items

---

## 📊 Analysis Performed

### ✅ Basic Exploration:
- Total number of rows
- Null value checks across all columns
- Count of unique product categories
- Stock status analysis (in-stock vs out-of-stock)

### ✅ Business Insights:
1. **Top 10 Best Value Products**  
   Based on highest discount percentages

2. **High MRP But Out of Stock**  
   Identify products that are premium but unavailable

3. **Estimated Revenue by Category**  
   Using `discountedSellingPrice × availableQuantity`

4. **MRP > ₹500 and Low Discount (<10%)**  
   Detect premium products that are not deeply discounted

5. **Top 5 Categories with Highest Avg Discount**

6. **Price per Gram for Products > 100g**  
   Helps evaluate best value in terms of pricing

7. **Weight Category Segmentation**  
   Classified as:
   - Low (<1kg)
   - Medium (1–5kg)
   - Bulk (>5kg)

8. **Total Inventory Weight per Category**

---

## 📌 Technologies Used

- SQL (PostgreSQL syntax)
- Relational database concepts
- Data cleaning + transformation
- Aggregate and analytical SQL queries

---

## 📈 How to Use

1. Clone or download this repository
2. Use any SQL client (like pgAdmin, DBeaver, or BigQuery)
3. Load the `.sql` file to run queries step-by-step

---
