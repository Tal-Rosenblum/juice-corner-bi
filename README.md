# Juice Corner – BI & Analytics Project

End-to-end Business Intelligence project for a juice chain's ordering & delivery system: from a data warehouse to dashboards, statistical analysis and decision-support tools.
Team project, Business Intelligence Systems course, Ben-Gurion University (2026).

![Dashboard](images/dashboard.png)

## Business Questions
- Where should the chain open its next branch?
- How can delivery quality and customer retention be improved?
- How should a fixed coupon budget be allocated to maximize net profit?

## Data
Orders, deliveries, customers, products, branches and riders – July 2023 to June 2026.

## What We Built
- **Data Warehouse** – Star schema with two fact tables (order items, deliveries) and a Type 2 slowly changing customer dimension.
- **Tactical Report** – Delivery quality and retention KPIs (On-Time Rate, Perfect Order Rate, Repeat Purchase Rate) by branch.
- **Strategic Report** – Expansion analysis using custom KPIs (Same-Store Revenue Gain, City Demand Index, New Branch Performance Ratio).
- **Digital Dashboard** – Management overview with KPI thresholds and drill-down pages.
- **OLAP Tool** – Flexible pivot analysis across 14 dimensions, with slice, dice, drill-down and roll-up.
- **Statistical Analysis (R + Tableau)** – Welch t-test, one-way ANOVA and linear regression on delivery delays.
- **Recommendation System (Python)** – Personalized product recommendations for repeat customers, validated on a chronological train/test split against a popularity baseline.
- **Coupon Budget Optimizer (Excel)** – Integer linear programming (knapsack) model solved with OpenSolver, with VBA-automated sensitivity analysis.

## Key Findings
- Recommended **Rampura** as the next branch location.
- Each minute of delay lowers customer satisfaction by ~0.04 points (p < 0.001).
- Vehicle type has no significant effect on delays – the issue is network-wide, not local.

## Tools
Tableau · R · Python (Google Colab) · Excel · OpenSolver · VBA

## Files
- [Full project report (Hebrew)](docs/report.pdf)
- `tableau/` – Tableau workbook
- `excel/` – Coupon optimizer
