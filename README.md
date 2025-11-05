# Executive Performance Dashboard - Power BI

## High-Level Sales and Profitability Analysis

This repository contains the dataset and Power BI report file (`.pbix`) for an Executive Performance Dashboard. The dashboard is designed to provide C-level executives with a high-level, interactive overview of key business performance metrics, focusing on sales, profitability, and regional performance.

The data model follows a classic star schema, enabling efficient analysis and drill-down capabilities. It integrates sales transactions (facts) with multiple lookup tables (dimensions) for customers, products, regions, and dates.

## Dashboard Features

* **KPI Monitoring:** Tracks core metrics such as Total Revenue, Total Profit, Profit Margin, and Total Units Sold.
* **Geographical Analysis:** Visualizes sales and profit distribution by country and region, allowing executives to identify top-performing and underperforming markets.
* **Product & Category Performance:** Analyzes revenue and profitability by product category (Audio, Security, Lighting, HVAC) to understand product mix performance.
* **Customer Insights:** Segments performance by customer type (Individual vs. Business) to track acquisition and profitability trends.
* **Time Series Analysis:** Includes trend lines for revenue and profit over time (by month, quarter, and year) to identify seasonality and growth patterns.

## Data Model

The analysis is based on a star schema consisting of one fact table and four dimension tables:

* **Fact Table:**
    * `Fact_Sales.csv`: Contains transactional data, including OrderID, UnitsSold, TotalRevenue, TotalCost, and Profit. This table links all dimensions.
* **Dimension Tables:**
    * `Dim_Customer.csv`: Provides customer-level details, including `CustomerKey` and `CustomerType`.
    * `Dim_Product.csv`: Contains product information, such as `ProductKey`, `ProductName`, and `ProductCategory`.
    * `Dim_Region.csv`: Includes geographical data like `RegionKey`, `RegionName`, `Country`, and `MonthlySalesTarget`.
    * `Dim_Date.csv`: A comprehensive date table for robust time-based analysis (Year, Quarter, Month, etc.).

## Technologies Used

* **Primary Tool:** Microsoft Power BI Desktop
* **Data Source:** CSV Files
* **Data Modeling:** Power Query (for ETL)
* **Analysis:** DAX (Data Analysis Expressions) for creating measures and calculated columns.

![Main Dashboard](https://github.com/devray11/Executive-Performance-Dashboard/blob/45ed95e3c3bad4132e84f12747fd724f9b420b76/Output-Image-Main-Dashboard.png)

![Side Dashboard](https://github.com/devray11/Executive-Performance-Dashboard/blob/45ed95e3c3bad4132e84f12747fd724f9b420b76/Output-Image-Side-Dashboard.png)
