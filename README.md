# 📊 Sales Analysis Dashboard

## 🌟 Problem Statement
A consumer goods company spanning categories such as Electronics, Footwear, Clothing, Home Appliances, Accessories, Kitchenware, Bags, and Personal Care requires actionable insights into its sales, profit, and customer buying behavior. The goal is to empower business stakeholders with interactive, visual dashboards that spotlight product performance, regional demand, profitability, discount effectiveness, and order-level dynamics for informed decision making.

## 🚀 Project Overview
This project analyzes sales data from a hypothetical store using Power BI. The goal is to enable stakeholders to identify patterns, track performance, and make informed decisions. The process includes:
- **Data Profiling & Transformation:** Cleaned, merged, and transformed data using Power Query.
- **Interactive Dashboards:** Created highly interactive visualizations across six report pages.
- **Key Business Insights:** Derived actionable insights using calculated metrics and relationships.

## 📂 Dataset Details
**File Name:** `Store+Data.xlsx`

The dataset consists of four sheets:
- **Dim Customers:** Customer details (`Customer ID`, `Customer Name`, `City`, `State`, `Pincode`, `EmailID`, `Phone Number`)
- **Dim Product:** Product details (`ProductID`, `Product Name`, `Product Line`, `Price Per Unit (INR)`)
- **Dim Promotion:** Promotion details (`PromotionID`, `Promotion Name`, `Ad Type`, `Coupon Code`, `Price Reduction Type`, `Percentage`)
- **Fact Table:** Order details (`OrderID`, `Date`, `CustomerID`, `PromotionID`, `ProductID`, `Units Sold`, `Price Per Unit`, `Total Sales`, `Discount Percentage`, `Discount Value`, `Net Sales`, `Profit`)

## 🔧 Data Transformation

### Key Steps
1. **Index Column:** Added `OrderID` as a unique identifier starting from 1.
2. **Merging Queries:** Joined fact table with dimension tables to enrich data.
3. **Calculated Columns:**
    - `Total Sales` = `Units Sold` * `Price Per Unit`
    - `Discount Value` = calculated using `Discount Percentage`
    - `Net Sales` = `Total Sales` - `Discount Value`
    - `Profit` = `Net Sales * 10%` (assumed)
4. **Data Profiling:** Ensured data quality by handling null values and duplicates.
5. **Relationship Setup:** Established one-to-many relationships for smooth interaction between tables.

## 📊 Report Pages & Visualizations

### 1. Start
- **Purpose:** Introduces the project and provides a "Start" button for navigation to the Overview page.

### 2. Overview
- **Visuals:**
    - **Cards:** Summarize Total Customers, Total Orders, Total Units Sold, Average Net Sales.
    - **Clustered Bar Chart:** Highlights average discount by promotion categories.
    - **Map:** Displays net sales by state (bubble size = sales volume).
    - **Donut Chart:** Shows total orders by product line.
    - **Scatter Plot:** Examines relationship between Sales and Profit.
    - **Stacked Column Chart:** Identifies top 3 customers by highest sales.
    - **Line Chart:** Depicts sales trends over time, with drill-down.
    - **Slicer:** Allows filtering by product names.

### 3. Trends
- **Line Charts:** Visualize net sales trends across daily, monthly, quarterly, and yearly intervals.

### 4. Product Analysis
- **Stacked Bar Charts:**
    - Show top 5 products by Sales, Quantity, and Profit.
    - Highlight bottom 5 products by the same metrics.

### 5. Dynamic Comparison
- **Date Slicers:** Compare metrics across two selected periods.
- **Bar Charts:** Display Total Sales, Total Profit, and Total Quantity for each period.

### 6. Detailed Breakdown
- **Table:** Comprehensive transactional data view.
- **Slicers:** Filter data by Date, Customer ID, Product Name, Promotion Name, City.
- **Custom Measure:** Ensures dynamic filtering via slicers.

---

## 🌟 Key Insights

- **Top Products:** Identified top and bottom performing products by sales, quantity, and profit.
- **Promotion Effectiveness:** Analyzed impact of discounts and promotions.
- **Customer Trends:** Highlighted top-performing customers by sales.
- **Geographic Insights:** States and cities driving the most sales.
- **Sales Trends:** Examined sales trends over time.
- **Dynamic Comparisons:** Performance tracked across different time periods.

---

## 📁 Files

- `Store+Data.xlsx`: Raw dataset.
- `Sales Analysis.pbix`: Power BI file including all transformations and visualizations.

---

## 🛠 How to Run the Project

1. Download `Store+Data.xlsx` and `Sales Analysis.pbix`.
2. Open the `.pbix` file in Power BI Desktop.
3. Refresh the data source to reconnect with the dataset.
4. Explore the interactive dashboards and uncover insights.

---

## 🤝 Contributions

Suggestions and contributions are welcome! If you have ideas to improve the dashboard or add features, please raise an issue or submit a pull request.
