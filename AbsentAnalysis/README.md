# MegaMart Absent Analysis Dashboard

## Overview
This dashboard provides a comprehensive analysis of absence metrics for MegaMart employees. It includes various visualizations and data points to help understand trends, frequency, and reasons for employee absences.
![AbsentAnalysisReport](https://github.com/rnkouser/PowerBI-Projects/blob/main/AbsentAnalysis/AbsentAnalysisReport.png)<br><br><br>

![AbsentAnalysisDrillthrough](https://github.com/rnkouser/PowerBI-Projects/blob/main/AbsentAnalysis/AbsentAnalysisDrillthrough.png)


## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Key Metrics](#key-metrics)
- [Visualizations](#visualizations)
- [Database Schema](#database-schema)
- [Data Insights](#data-insights)
- [Usage](#usage)


## Introduction
This dashboard is designed to offer detailed insights into the absence metrics of MegaMart employees. It helps HR managers and analysts monitor and manage employee absences, identify trends, and make informed decisions to optimize workforce productivity and well-being.

## Features
1. **Period Selection**:
   - Users can select the year (2015 - 2024) and the quarter (Q1, Q2, Q3, Q4) or specific months (Jan - Dec) to filter the data.
   
2. **Filters**:
   - **Store Selection**: Filter data by different store locations.
   - **Absent Metrics**: Choose between different metrics such as the number of absences and average absent hours.

## Key Metrics
The report highlights the following key metrics:
- **Number of Absents**: 3M
- **Total Absents**: 13M
- **Average Absent Hour**: 4.00

## Visualizations
The dashboard includes various visualizations to provide insights into absence performance:

### Average Overtime Hour by Marital Status
A bar chart showing the average overtime hours for different marital statuses.

### Absent Trend
Displays the number of absents and total absent.

### Absent Frequency
Shows the average absent hour.

### Total Absent by Department
A bar chart showing total absents by department, with increases and decreases highlighted.

### Average Absent Hour by Date
A line chart showing the average absent hour over time from April 2023 to July 2023.

### Number of Absents by Employee Name and Category
A stacked bar chart showing the number of absents by employee name and category, with categories such as:
- Bereavement
- Child Care
- Emergency
- Hang Over
- Local Disorder
- Medical Appointment
- Sick
- Traffic

### Employee Absence Data
A table listing employee names and their absence data across different stores (AliquidStores) with varying absence counts:
- **Employee Names**: 
  - AliquidStores - 37
  - AliquidStores - 474
  - AliquidStores - 512
  - AliquidStores - 667
  - AliquidStores - 674
  - AliquidStores - 727
  - AliquidStores - 859
  - AliquidStores - 895
- **Total Absence Counts**: 
  - 15742
  - 16152
  - 15618
  - 15610
  - 16534
  - 15208
  - 16350
  - 16082

## Database Schema
The following schema outlines the structure of the database used for this dashboard, showing how different tables are interconnected to store and manage data related to employee absences:

### Schema Overview
The schema consists of five tables: Date, Absent Category, Employee, EDW Fact_HRAbsent, and Store. The relationships between these tables are indicated by lines connecting them.

### Diagram
![AbsentAnalysisModel](https://github.com/rnkouser/PowerBI-Projects/blob/main/AbsentAnalysis/AbsentAnalysisModel.png)

### Table Details
1. **Date Table**:
   - Fields: businessdatekey, businessday, businessquarter, businessWeekNo, Date, effectivedate, EnglishDayofWeek, Englishmonth, FrenchDayofWeek etc

2. **Absent Category Table**:
   - Fields: Category, CategoryID, CategorySK, EffectiveStartDate etc

3. **Employee Table**:
   - Fields: DateOfBirth, EffectiveEndDate, EffectiveStartDate, EmployeeID, EmployeeName, EmployeeNo, EmployeeSK, MaritalStatus etc

4. **EDW Fact_HRAbsent Table**:
   - Fields: Absent_CategorySK, Absent_DateSK, Absent_Hour, AbsentSK, EmployeeSK, LoadDate, StoreSK etc

5. **Store Table**:
   - Fields: City, EffectiveStartDate, Product, State, Store, StoreID, StoreSK, StreetAddress etc

### Relationships
- The **Date** table is connected to the **EDW Fact_HRAbsent** table via

## Data Insights
- **Top Absent Departments**: Insights into which departments have the highest and lowest total absents.
- **Absent Trends**: Analysis of how absent hours fluctuate over time.
- **Categories of Absents**: Breakdown of different types of absences by employee.
     
## Usage:
  This dashboard is useful for HR managers and analysts to monitor and manage employee absences, identify trends, and make informed decisions to optimize workforce productivity and well-being. ## Contact For any queries or support, 
