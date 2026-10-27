# HR Analytics Dashboard | Power BI

An interactive Power BI report analyzing HR data to understand workforce structure, employee performance, and key people metrics.

## Overview

This is my first end-to-end Power BI project. It covers cleaning the raw HR dataset, building a data model, writing DAX measures, and designing a dashboard around HR KPIs.

## What I Did

**1. Data Cleaning (Power Query)**
- Found and fixed data quality issues before modeling
- Kept `StockOptionLevel` as Text since it is used as a category, not for calculations
- Created a custom column `RatingGap` = `SelfRating - ManagerRating` to compare how employees see themselves versus how their managers rate them

**2. Data Modeling**
- Linked the `Employee` table (one row per employee) to the `PerformanceRating` table (multiple rows per employee) on `EmployeeID`
- Relationship: one-to-many (1 → *), no bridge table needed
- Used `ManagerRating` as the main rating dimension

**3. DAX Measures and KPIs**
- Built measures for core HR KPIs, each documented and explained

**4. Dashboard**
- Visuals connected through the model with no relationship errors

## Tools

- Power BI Desktop
- Power Query
- DAX

## Team Project 

| 1 | Ibrahem Ahmed Hafez Mahmoud |
| 2 | Mohamed Abdelmoneim Abdelhalim Abdelhafez |
| 3 | Azzam Hussein Ahmed Hussein Hussein |
| 4 | Mohamed Ayman Mohamed Aly |
| 5 | Mostafa Mohamed Mostafa Abdelsamie |
| 6 | Abdullah Hussein Abdelaziz Hussein |
