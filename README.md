Project Overview

This repository contains the full end-to-end Business Intelligence (BI) solution built using the AdventureWorksDW dataset.
The project includes data acquisition, cleaning, modeling, KPI definition, exploratory data analysis (EDA), dashboard development, and documentation.

The work references content from:

Implementation.pdf 

Implementation

System_Analysis_Design_Document.pdf 

System_Analysis_Design_Document

Project - Documentation.pdf 

Project - Documentation

 Key Features
🔹 1. Data Acquisition & Preparation

Imported FactInternetSales, FactResellerSales, and multiple dimension tables.

Cleaned missing values, standardized text fields, removed unused attributes, and optimized data types.

Merged Product Category + Subcategory for easier reporting.
(Implementation.pdf — Data Cleaning section, page 2–5)

🔹 2. Data Modeling (Star Schema)

Built a relational model connecting Fact tables to Dimensions through primary/foreign keys.

Ensured one-to-many relationships for correct filter propagation.
(Implementation.pdf — Data Modeling + ER diagram)

🔹 3. Business Logic (DAX Measures)

Examples:

Total Sales = SUM(FactInternetSales[SalesAmount])
Total Cost = SUM(FactInternetSales[TotalProductCost])
Total Profit = [Total Sales] – [Total Cost]
Profit Margin % = DIVIDE([Total Profit], [Total Sales])

🔹 4. Exploratory Data Analysis (EDA)

Identified insights such as:

Sales trends

Profitability by category

Customer demographics

Regional performance
(Implementation.pdf — EDA visuals on page 7)

🔹 5. Interactive Power BI Dashboard

Dashboard pages include:

Sales Overview

Product Performance

Customer Analysis

Geographical Analysis
(UI mockups and visuals: System Analysis & Design pages 8–10)

🔹 6. Requirements Engineering

Includes:

Functional Requirements (FR1–FR6)

Non-Functional Requirements (Performance, Accuracy, Usability…)
(System Analysis Document — pages 5–7)

🔹 7. Project Planning

Includes project proposal, scope, timeline, milestones, risk assessment, and KPIs.
(Project Management Document — pages 3–10)
Tools & Technologies

Power BI Desktop

Power Query (ETL)

DAX (Data Analysis Expressions)

AdventureWorksDW Database

Microsoft SQL Server

Excel / CSV (supplemental preprocessing)

📌 KPIs Included

As defined in project documentation:

✔ Sales KPIs

Total Sales Revenue

Average Order Value

Gross Profit Margin

✔ Customer KPIs

Retention Rate

CLV

New vs Returning Customers

 Product KPIs

Top Selling Products

Category Contribution %

 Regional KPIs

Sales by Territory

Country Revenue Growth

 Operational KPIs

Sales Growth Rate

On-Time Delivery Rate

 Project Timeline

From September 2025 → November 2025, including:

Data Cleaning

Data Modeling

Dashboard Development

Testing & Validation

Final Reporting

Full timeline and Gantt chart in Project Documentation.
(Project Plan — page 5)

 How to Use the Dashboard

Download the .pbix file from the repository.

Open using Power BI Desktop.

Ensure the AdventureWorksDW dataset is available if refreshing data.

Interact with slicers, filters, and drill-downs to explore insights.

 Team Roles

As defined in System Analysis Document (page 4):

Project Manager: Oversees progress

Data Engineers: Data collection & cleaning

Data Analysts: EDA & insights

BI Developers: Dashboard building & KPIs

Documentation Specialist: Reporting & system documentation
