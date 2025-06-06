📊 Financial Dashboard – Power BI Report

![image](https://github.com/user-attachments/assets/720a48ec-c155-4540-91b9-85601976b9b0)  ![image](https://github.com/user-attachments/assets/226ac802-6ccf-4a30-822b-afc4289dbfa7) ![image](https://github.com/user-attachments/assets/6eb86de2-c6c7-4e34-b9fb-6dab369d081c)





🔍 1. Purpose

This Power BI dashboard provides a real-time financial snapshot, helping stakeholders track revenue, expenses, profit, and budget performance — all in one place. The goal: enable fast, data-driven decisions.

👥 2. Audience

Senior Management

Department Heads

Analysts & Auditors

🧩 3. Data Sources
SQL Database – Core transactional data (Revenue, Expenses)

Excel (Budget) – Monthly/Yearly budget files

SharePoint – Manual entries & adjustments

🏗️ 4. Data Model
Fact Table: FactFinancials

Dimensions: Date, Department, Cost Center, Account

ETL: Power Query used for transformations & data cleaning

🔢 5. Key Metrics
Metric	DAX Measure (Simple Logic)
Total Revenue	SUM(Financials[Revenue])
Total Expenses	SUM(Financials[Expenses])
Net Profit	[Revenue] - [Expenses]
Budget Variance %	DIVIDE([Actual] - [Budget], [Budget])
Cumulative Revenue	CALCULATE([Revenue], DATESYTD(...))

📈 6. Visuals & Pages
Page	Visuals Used
Summary View	KPI Cards, Line Chart
Budget vs Actual	Column Chart, Slicer
Profit Trend	Waterfall, Area Chart
Cost Center View	Matrix, Bar Chart

🎯 7. Features
Slicers: Date, Department, Cost Center

Drill-through to department-level reports

Tooltips with YoY comparison

Dynamic alerts using conditional formatting


