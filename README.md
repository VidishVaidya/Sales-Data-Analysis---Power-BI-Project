# Sales Data Analysis-Dashboard

## Problem Statement

A consumer goods company spanning categories such as Electronics, Footwear, Clothing, Home Appliances, Accessories, Kitchenware, Bags, and Personal Care requires actionable insights into its sales, profit, and customer buying behavior. The goal is to empower business stakeholders with interactive, visual dashboards that spotlight product performance, regional demand, profitability, discount effectiveness, and order-level dynamics for informed decision making.


### Steps followed 

1. Data Validation
- Column Distribution, Profile, and Quality: Assessed each column for validity, consistency, and completeness to identify missing values or anomalies.

- Data Type Correction: Standardized data types (e.g., dates, numbers, strings) to ensure robust modeling and accurate visualizations.

2. Data Transformation
- Query Merging (Joins): Integrated multiple data tables (fact and dimension) via joins to establish a holistic data model.

- Column Removal: Eliminated unnecessary or redundant columns to streamline the dataset.

- Custom Calculations: Introduced calculated fields such as ‘Total Sales’ (Units Sold × Price per Unit).

- Null Value Handling: Replaced nulls with zeroes where appropriate for consistency and straightforward analysis.

3. Data Modeling
- Primary & Foreign Key Setup: Defined PKs and FKs with correct data types to ensure integrity. All relationships maintained one-to-one, one-to-many, or many-to-one cardinality as needed.

- Star Schema Design: Implemented a star schema separating the fact table (sales transactions) and relevant dimension tables (products, customers, dates, etc.).

- Model View: Established and visualized table relationships and cardinality in the model view for maintainability and transparency.

4. Report View and Visualizations

Requirement-specific Visuals:

- Bar Charts: For top/bottom 5 products by sales/profit/quantity sold.

- Line Charts: To illustrate sales trends across daily, monthly, quarterly, and annual periods.

- Scatter Plots: To show the relationship between net sales and profit, revealing cases where high sales may not yield high profits.

- Bar Charts: For analyzing average discount by discount category.

- Cards: To report total number of orders in an at-a-glance format.

- Map Visuals: To display sales data segregated by cities for regional performance analysis.

- Tables with Dynamic Filtering: Offered comprehensive order-level views filterable by product, date, customer ID, or promotion category.

- User-driven Period Comparison: Enabled comparison of sales, profit, and quantity sold between arbitrary user-selected time frames via DAX measures (e.g., CALCULATE, SUM, USERELATIONSHIP) and interactive slicers.

- Leveraged visual, page-level, and report-level filters to sharpen focus and enhance interactivity.


## Insights Gathered
- Product Performance: Identified the strongest and weakest products, spotlighting areas for promotion or improvement.

- Sales Trends: Uncovered seasonal and periodic patterns in sales, helping management plan for peak demand and lean periods.

- Profitability Analysis: Mapped the relationship between high revenue and actual profit, supporting better pricing and discount strategies.

- Regional Opportunities: Visualized sales by city, uncovering high-performing regions and highlighting areas with growth potential.

- Discount Effectiveness: Analyzed whether specific discount categories boost sales or erode profit, guiding future discounting strategies.
