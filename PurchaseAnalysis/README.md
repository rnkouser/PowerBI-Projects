# MegaMart Purchase Analysis Report

## Overview
This report provides a comprehensive analysis of MegaMart's purchase transactions over the years. It includes detailed insights into transaction purchase amounts, delivery purchase amounts, order purchase amounts, and the number of transactions. The report is designed to help stakeholders understand purchasing trends, compare different metrics, and make informed decisions based on the data.

![Star Schema](https://github.com/rnkouser/PowerBI-Projects/blob/main/PurchaseAnalysis/PurchaseAnalysisReport.png)<br><br><br>

![Star Schema](https://github.com/rnkouser/PowerBI-Projects/blob/main/PurchaseAnalysis/PurchaseAnalysis-Drillthrough.png)


## Table of Contents
- [Introduction](#introduction)
- [Key Metrics](#key-metrics)
- [Filters](#filters)
- [Visualizations](#visualizations)
- [Star Schema](#star-schema)


## Introduction
This report is designed to provide comprehensive insights into MegaMart's purchasing performance across various dimensions such as time, store, promotion, and product. The interactive dashboards allow users to filter data and gain detailed insights.

## Key Metrics
The report highlights the following key metrics:
- **Transaction Purchase Amount**: 5.47bn
- **Delivery Purchase Amount**: 5.64bn
- **Order Purchase Amount**: 5.47bn
- **Transaction Number Purchases**: 22K

## Filters
The report includes several data filters to allow users to narrow down the analysis:
- **Select Period**: Options for 2015 to 2024.
- **Quarter Selection**: Q1, Q2, Q3, Q4.
- **Month Selection**: Jan. - Dec.
- **Store Selection**: Dropdown to select specific stores.
- **Promotion Selection**: Dropdown to select specific promotions.

## Visualizations
The report includes various visualizations to provide insights into purchasing performance:

### Top 5 Products by Purchase Transactions
Bar chart showing the top 5 products with their purchase transaction amounts:
- **Always...**: 0.15bn
- **Aveen...**: 0.13bn
- **Axen...**: 0.13bn
- **Azed...**: 0.14bn
- **Caldr...**: 0.14bn

### Detailed Analysis
#### Transaction Purchase Amount by Date
Line graph showing transaction purchase amounts over time from Jan 2024 to Jul 2024, with key points at 80M, 72M, 69M, 50M, 36M, 42M, 46M, 17M.

#### Transaction Purchase Amount by State
Map of the United States showing transaction purchase amounts by state, with different states highlighted in various colors.

### Flow Analysis
Detailed flow chart showing the breakdown of transaction purchase amounts by store, department, product, and employee name:
- **Store**: Cupidcoffee - 148
- **Department**: Computer & Electronics
- **Product**: Samsung Galaxy Tab A
- **Employee Name**: MAXIMILLIAN, Mendez

## Star Schema
### Schema Overview
The star schema for this report illustrates the relationships between the fact table and dimension tables, designed to optimize query performance and improve data retrieval speed.

### Diagram
![Star Schema](https://github.com/rnkouser/PowerBI-Projects/blob/main/PurchaseAnalysis/PurchaseAnalysis-StarSchema.png)

### Schema Details
- **Fact Table**: EDW factsales
  - Contains measurable, quantitative data.
- **Dimension Tables**:
  - **Store**: Contains store-related attributes.
  - **Employee**: Contains employee-related attributes.
  - **POSChannel**: Contains point-of-sale channel attributes.
  - **Product**: Contains product-related attributes.
  - **Business Year**: Contains business
