# powerbi-financial-performance-dashboard
Executive-level Power BI dashboard for financial performance, variance analysis, and forecasting

**Project Overview**

This project demonstrates an end-to-end Power BI solution designed to support executive decision-making through financial performance analysis.
The dashboard covers Actual vs Budget, Forecast accuracy, variance analysis, profitability drivers, and scenario modeling, simulating how a BI developer works in real-world enterprise environments.
The solution focuses on clean data modeling, advanced DAX, and business storytelling, not just visuals.

**Data Model & Architecture**

Star schema design with fact and dimension tables

Dedicated Date table created using DAX and marked as a Date table

Disconnected Scenario table used for what-if analysis

Single-direction, one-to-many relationships for performance optimization

**Key Tables:**

Fact_Financials

Dim_Date

Dim_Region

Dim_Account

Scenario (Disconnected)

**Dashboard Pages & Business Use Cases**

**Page 1 — Executive P&L Overview**

**Purpose**: High-level financial snapshot for leadership

**Key Metrics**:

Total Actual Revenue

Total Budget Revenue

Revenue Variance & Variance %

Executive insight summary

**Highlights**:

Month-over-month revenue trends

Regional variance contribution

Clear executive insights explaining why performance changed

**Page 2 — Variance & Driver Analysis**

**Purpose**: Identify what drives over- or under-performance

**Key Analysis**:

Revenue variance by account type (Revenue, OPEX, COGS)

Top variance drivers

Actual vs Budget trend analysis

**Advanced Logic**:

Signed variance logic for OPEX (positive variance = negative business impact)

Driver-level filtering for targeted analysis

**Page 3 — Profitability Analysis**

**Purpose**: Understand margin performance across dimensions

**Key Metrics**:

Revenue

Gross Profit

Gross Margin %

COGS % of Revenue

Insights Enabled:

High vs low margin regions

Cost impact on profitability

Margin trends over time

**Page 4 — Forecast & Scenario Analysis**

**Purpose**: Support planning and strategic decision-making

**Key Metrics**:

Total Actual vs Total Forecast

Forecast Accuracy %

Forecast Variance

Advanced Features:

Actual vs Forecast trend analysis

Forecast variance by year

Scenario modeling using a disconnected table

What-if revenue uplift scenarios

**Key DAX Measures** (Examples)

Total Actual Revenue =
SUM(Fact_Financials[ActualAmount])

Revenue Variance =
[Total Actual Revenue] - [Total Budget Revenue]

Forecast Accuracy % =
1 - DIVIDE(ABS([Forecast Variance]), [Total Forecast])

Gross Margin % =
DIVIDE([Gross Profit], [Revenue])


**Advanced techniques used**:

SWITCH

SELECTEDVALUE

Time intelligence (YTD, YoY)

Scenario-based measures

Signed variance logic

**Business Value Delivered**

Enables executives to track financial performance vs plan

Highlights key cost and revenue drivers

Improves forecast reliability analysis

Supports scenario-based decision-making

Translates raw financial data into actionable insights

**Tools & Technologies**

Power BI Desktop

DAX

Power Query

Star Schema Data Modeling

Financial & FP&A concepts

**Dashboard Screenshots**

<img width="866" height="483" alt="image" src="https://github.com/user-attachments/assets/c2d91917-cf94-4aae-992d-89a32f693a94" />


<img width="875" height="488" alt="image" src="https://github.com/user-attachments/assets/4e082fd9-6db2-4847-a11d-ddc1ea454a07" />

<img width="871" height="484" alt="image" src="https://github.com/user-attachments/assets/efb48bc8-ad9a-4215-9261-8d7e6d04895c" />

<img width="867" height="486" alt="image" src="https://github.com/user-attachments/assets/d154427c-79ab-4313-9913-dd33ba9475bf" />

**Key Skills Demonstrated**


Executive dashboard design

Financial data modeling

Advanced DAX & time intelligence

Variance and profitability analysis

Forecasting & scenario modeling

Business storytelling with data

**How This Project Is Used**

This project is part of my professional Business Intelligence portfolio and demonstrates how I design and deliver executive-level Power BI dashboards in real business environments, with a strong focus on clarity, performance, and actionable insights.

**Author**

**Kalyan Raj**

Business Intelligence / Power BI Developer







