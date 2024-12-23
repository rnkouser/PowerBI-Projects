# 🐔 Falanza Agro-Allied Limited Egg Production Dashboard

## Overview
This Power BI dashboard provides an in-depth analysis of egg production, mortality, feeding, and associated costs for Falanza Agro-Allied Limited. The goal is to identify trends, optimize production, and manage costs effectively.

## Table of Contents
- [Introduction](#introduction)
- [Deliverables](#deliverables)
- [Key Metrics](#key-metrics)
- [Visualizations](#visualizations)
- [Data Insights](#data-insights)
- [Database Schema](#database-schema)
- [Usage](#usage)


## Introduction
Falana Lora, the CEO of Falanza Agro-Allied Limited, is deeply concerned with the inconsistency in egg production of 36,000-layer birds, daily mortality records in the four pen houses, rising feed costs, and other expenses compared to revenues. Additionally, the market oversupply of eggs by Obasanjo Farm Limited and other large-scale poultry farms has led to a fall in market sales of eggs.

Falanza suspects that employee activities, such as feeding time, feeding methods, and medication, may contribute to high mortality and low production rates. Daily egg collection, mortality, and feeding data for 5 years are available, stored in Microsoft Excel due to budget constraints.

## Deliverables
Using Power BI, the following deliverables are required:
1. **Replicate the Egg Collection, Mortality, Feeding Sheet**: Create a Power BI report replicating the provided Excel sheets for egg collection, mortality, and feeding.
2. **Monthly Revenue Analysis**: Analyze monthly revenue from egg sales, mortality, and feeding. Mortality costing is calculated based on the price of a crate of eggs and the current market price of a bird.
3. **Trend Analysis of Egg Production**: Conduct trend analysis and forecasting of egg production to advise on bird disposition based on the age of laying.
4. **Mortality Rate Analysis**: Analyze mortality rates based on events such as pecking, accidents, and stampedes.
5. **Feeding and Costing Analysis**: Provide weekly, monthly, and yearly feeding and costing analysis.

## Key Metrics
- **Total Egg Production**: Overview of egg production over the 5-year period.
- **Daily Mortality Rate**: Records of daily bird mortality in the four pen houses.
- **Feeding Costs**: Analysis of weekly, monthly, and yearly feeding costs.
- **Revenue from Egg Sales**: Monthly revenue generated from egg sales.
- **Mortality Cost**: Cost incurred due to bird mortality.

## Visualizations
The dashboard includes various visualizations to provide insights into egg production and related metrics:

### 📈 Egg Production Trend
Line chart showing egg production trends over the 5-year period.

### 💀 Mortality Rate by Event
Bar chart displaying mortality rates categorized by events such as pecking, accidents, and stampedes.

### 💸 Revenue Analysis
Pie chart breaking down revenue from egg sales, feeding costs, and mortality costs.

### 🐣 Feeding Cost Analysis
Stacked bar chart showing weekly, monthly, and yearly feeding costs.

### 🐓 Bird Disposition Forecast
Forecasting graph advising bird disposition based on the age of laying.

## Data Insights
- **Production Trends**: Insights into the consistency and fluctuations in egg production.
- **Mortality Causes**: Analysis of the primary causes of bird mortality and their impact on production.
- **Cost Management**: Evaluation of feeding costs and their correlation with production and mortality rates.
- **Revenue Optimization**: Strategies for optimizing revenue through improved production and cost management.

## Database Schema
The following schema outlines the structure of the database used for this dashboard, showing how different tables are interconnected to store and manage data related to egg production and associated metrics:

### Schema Overview
The schema consists of tables for egg collection, mortality, feeding, and revenue, connected by unique identifiers such as date and bird ID.

### Table Details
1. **Egg Collection Table**:
   - Fields: Date, PenHouse, TotalEggsCollected, AverageEggsPerBird

2. **Mortality Table**:
   - Fields: Date, PenHouse, MortalityCount, CauseOfDeath

3. **Feeding Table**:
   - Fields: Date, PenHouse, FeedType, FeedAmount, FeedingCost

4. **Revenue Table**:
   - Fields: Date, PenHouse, TotalEggSales, MortalityCost, NetRevenue

### Relationships
- The **Egg Collection** table is connected to the **Mortality** and **Feeding** tables via the **Date** field.
- The **Revenue** table is connected to the **Egg Collection**, **Mortality**, and **Feeding** tables via the **Date** field.

## Usage
This dashboard is useful for managers and analysts at Falanza Agro-Allied Limited to monitor and manage egg production, identify trends, and make informed decisions to optimize production and reduce costs.

