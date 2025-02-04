
# Amazon Sales Analysis - Tableau Project

## Overview

This Tableau project analyzes Amazon sales data to provide insights into revenue, profit, shipments, and order trends. The dashboard is structured to give executives and analysts a clear understanding of sales performance across various dimensions. The analysis covers key metrics such as revenue, profit, shipments, and order fulfillment, helping businesses optimize their sales strategy and operations.

## Data Sources

The workbook connects to a federated data source:

Source: <a href="https://github.com/gsinghpawar25/Data-Analysis-DB-AmazonSalesInsight-Proj2/blob/main/Amazon%20Sales%20data_Amazon%20Sales%20data.csv">Data Source</a>

Multiple references: The same data source is referenced multiple times throughout the workbook.

Data Fields: Includes key fields such as Order ID, Customer ID, Product Category, Sales Amount, Order Date, Ship Date, and Profit etc.

## Worksheets

The following worksheets are included in the Tableau workbook, each focusing on different aspects of sales and operational performance:

#### Cost Split 
- Breakdown of costs associated with sales and operations.

#### Orders Split
- Analysis of orders based on various parameters.

#### Orders each year
- Year-wise distribution of orders.

#### Priority wise orders
- Segmentation of orders based on priority levels.

#### Profit Country wise
- Profit distribution across different countries.

#### Profit Region wise
- Regional profit insights.

#### Profit Split
- Analysis of profit margins across different categories.

### Revenue
- Overall revenue trends and performance.

#### Revenue Split
- Revenue breakdown by different dimensions.

### Sales Channel Analysis
- Performance analysis of various sales channels.

#### Shipment Days
- Analysis of delivery and shipment timelines.

#### Shipments cost per year
- Yearly breakdown of shipment costs.

### Total profit
- Overall profit trends.

### Total revenue
- Overall revenue trends.

#### Units Sold
- Analysis of total units sold.

## Dashboards

The workbook includes the following interactive dashboards to facilitate data visualization and insights:

Tableau Workbook: <a href="https://public.tableau.com/app/profile/gyanendra.singh.pawar/viz/AmazonSalesAnalysis-Proj2/SplitAnalysis?publish=yes">Workbook</a>

## Amazon - Home Page -
A high-level overview of key sales metrics and performance.
![Amazon home page](https://github.com/user-attachments/assets/236f4ca9-40df-4c34-9c12-f905b831726f)


## Executive Page - 
Designed for executives to quickly grasp business performance.
![Amazon executive page](https://github.com/user-attachments/assets/714d0643-c39a-440a-932e-2b11455ba089)


## Revenue Analysis - 
Detailed revenue trends and breakdown.
![Amazon Revenue Analysis](https://github.com/user-attachments/assets/0469b9ed-7ffc-4946-969f-21f3b458a25a)


## Split Analysis - 
Detailed breakdown of sales, revenue, and profit.
![Amazon Split analysis](https://github.com/user-attachments/assets/8c20336e-e9d7-4611-8733-6b9b9dc516fa)


### Calculated Fields

The following calculated fields are used within the workbook to derive key insights:

-- [Total Revenue] - [Total Cost] (Profit Calculation)

-- DATEDIFF('day', [Order Date], [Ship Date]) (Shipping Time Calculation)

-- if SUM([Total Revenue]) = WINDOW_MAX(SUM([Total Revenue])) then 'color' else 'no color' end (Conditional Highlighting for Revenue)

-- COUNT([Order ID]) (Order Count Calculation)

-- Additional calculations for revenue trends, profit analysis, and order segmentation.

## Key Insights Provided

-- Revenue and Profit Trends: Analysis of revenue and profit split across regions, categories, and channels.

-- Order Distribution: Yearly and priority-wise order breakdown, identifying trends in customer purchasing behavior.

-- Shipping Analysis: Shipment cost, days taken for shipment, and order delivery trends to optimize logistics.

-- Executive Dashboard: A high-level overview of business performance for stakeholders, enabling data-driven decision-making.

-- Sales Channel Performance: Evaluation of different sales channels to determine the most effective distribution methods.

-- Customer Insights: Understanding customer purchase behavior, order priorities, and product preferences.

## Usage

Open the Tableau workbook (.twb) in Tableau Desktop.

Navigate through the dashboards for insights.

Use filters, drill-down options, and interactive features to explore the data in depth.

Compare year-over-year sales trends and segment data by region, category, or priority.

## Author

This project was created to analyze Amazon's sales data and derive meaningful insights using Tableau, helping businesses optimize their strategies and drive growth. For further details conatact author : singhpawargyanendra@gmail.com
