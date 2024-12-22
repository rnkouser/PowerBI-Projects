# MegaMart Sales Analysis Report

## Overview
Welcome to the MegaMart Sales Analysis Report!
This project provides an in-depth analysis of MegaMart's sales performance over the years. Using Power BI, the report offers interactive visualizations and key metrics to help understand transaction sales, delivery sales, order sales, and transaction numbers.

![SalesAnalysisReport](https://github.com/rnkouser/PowerBI-Projects/blob/main/SalesAnalysis/SalesAnalysisReport.png)<br><br><br>

![SalesAnalysisDrillthrough](https://github.com/rnkouser/PowerBI-Projects/blob/main/SalesAnalysis/SalesAnalysis-Drillthrough.png)

## Table of Contents
- [Introduction](#introduction)
- [Key Metrics](#key-metrics)
- [Filters](#filters)
- [Visualizations](#visualizations)
- [Star Schema](#star-schema)
- [Usage Instructions](#usage-instructions)


## Introduction
This report is designed to provide comprehensive insights into MegaMart's sales performance across various dimensions such as time, store, promotion, and product. The interactive dashboards allow users to filter data and gain detailed insights.

## Key Metrics
The report highlights the following key metrics:
- **Transaction Sales Amount**: $318.69M
- **Delivery Sales Amount**: $719.13M
- **Order Sales Amount**: $318.69M
- **Transaction Number Sales**: 206K

## Filters
The report includes several data filters to allow users to narrow down the analysis:
- **Select Period**: Options for 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023, 2024 Q1, Q2, Q3, Q4, Jan, Feb, Mar, Apr, May, Jun,Jul, Aug,Sep, Oct, Nov, Dec.
- **Store**: Dropdown to select specific stores.
- **Promotion**: Dropdown to select specific promotions.

## Visualizations
The report includes various visualizations to provide insights into sales performance:

### Top 5 Products by Sales Transactions
Bar chart showing sales for the top 5 products:
- **Dell Ins.**: $0.14bn
- **Samsung**: $0.11bn
- **Monotox**: $0.11bn
- **Switz**: $0.08bn
- **Gerber**: $0.08bn

### Sales Comparison Analysis
Sankey diagram showing the flow of transaction sales amount through different stores, departments, products, and employees. Example:
- **Store**: Cupidcoffee - $1,146,894.81
- **Department**: Computer & Electronics - $2,122,532.06
- **Product**: Samsung Galaxy Tab A - $808,985.38
- **Employee**: ASHER, Chang - $528,028.00

### Sales Trend Analysis
#### Transaction Sales Amount by Date
Line chart showing sales trends over time with notable points:
- Peak at $13.2M in May 2024
- Drop to $0.3M in Mar 2024

#### Transaction Sales Amount by State
Map showing sales distribution across different states.

### Usage Instructions
- Navigating the Report: Use the tabs at the top to switch between different analysis reports.
- Filtering Data: Use the filters on the left to narrow down the data by period, store, and promotion.
#### Interpreting Visuals:
- The bar chart provides a quick view of the top-selling products.
- The Sankey diagram helps trace the flow of sales through various categories.
- The line chart shows sales trends over time, helping identify peaks and troughs.
- The map visualizes sales distribution geographically.

  ## Star Schema
### Schema Overview
The star schema for this report illustrates the relationships between the fact table and dimension tables, designed to optimize query performance and improve data retrieval speed.

![Star Schema](https://github.com/rnkouser/PowerBI-Projects/blob/main/SalesAnalysis/SalesAnalysis-StarSchema.png)

### Schema Details
- **Fact Table**: EDW factsales
  - Contains measurable, quantitative data.
- **Dimension Tables**:
  - **Store**: Contains store-related attributes.
  - **Employee**: Contains employee-related attributes.
  - **POSChannel**: Contains point-of-sale channel attributes.
  - **Product**: Contains product-related attributes.
  - **Business Year**: Contains business year attributes.
  - **Date**: Contains date-related attributes.
  - **Customer**: Contains customer
