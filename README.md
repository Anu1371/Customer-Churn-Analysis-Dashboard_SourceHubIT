📊 Customer Churn Dashboard – README
📝 Overview

This Power BI dashboard helps analyze customer churn (customers who left vs. active).
It shows KPIs, charts, and filters to understand churn patterns across time, region, plan, and gender.

⚙️ How it Works
1. Data Source

Data is imported into Power BI from an Excel/CSV file.

Key columns used:

CustomerID

Status (Active / Churned)

Region

Plan (Basic, Premium, Standard)

Gender

MonthlyRevenue

ChurnDate

2. DAX Measures Created

To calculate KPIs:

Total Customers = DISTINCTCOUNT(CustomerID)

Churned Customers = count of Status = "Churned"

Churn Rate % = (Churned Customers ÷ Total Customers) × 100

Total Monthly Revenue = SUM(MonthlyRevenue)

Revenue Lost = SUM(MonthlyRevenue where Status = "Churned")

3. KPIs (Top Row)

The top row shows 5 key metrics in card visuals:

Total Customers

Churned Customers

Churn Rate (%)

Revenue Lost ($)

Total Monthly Revenue ($)

4. Charts (Middle Section)

Line Chart (Churn by Month) → Shows churn trend over time.

Bar Chart (Churn by Region) → Compares churn across regions.

Donut Chart (Churn by Gender) → Splits churn by gender.

5. Filters (Bottom Section – Slicers)

Interactive filters (slicers) allow users to focus on:

Status → Active vs Churned

Region → North, South, East, West

Plan → Basic, Premium, Standard

👉 Selecting a filter will update all KPIs and charts dynamically.

6. Design Layout

Top row → KPIs (cards).

Middle row → Trend chart + donut chart.

Bottom row → Regional chart + slicers.

Title → “Customer Churn Dashboard” at the top.

🎯 How to Use the Dashboard

Open Power BI file (.pbix).

Use slicers (right side) to filter by status, region, plan.

Hover over charts to see details (tooltips).

Watch KPIs update instantly when you change filters.

📌 Insights You Can Get

What % of customers are churned.

How churn changes month by month.

Which region has the highest churn.

Which plan type churns the most.

Revenue loss due to churn.
