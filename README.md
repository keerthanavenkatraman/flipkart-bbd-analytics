# Flipkart Big Billion Days — Regional Performance Analysis

## Project Overview
This project analyses Big Billion Days sales performance using SQL, Excel, and Tableau Public. It focuses on completed-order revenue, regional performance, product categories, and monthly trends.

## Tools Used
- SQL for querying and analysing the data
- Microsoft Excel for data cleaning, reconciliation, and PivotTables
- Tableau Public for interactive dashboards
- Notepad for project documentation

## Key Performance Indicators
- Completed-order revenue: ₹346,200
- Completed orders: 63
- Units sold: 106

## Key Findings
1. Total completed-order revenue was ₹346,200 across 63 completed orders.
2. Electronics generated ₹142,300, representing approximately 41.1% of completed-order revenue.
3. North generated ₹119,300, with a 22.8% revenue decrease from September to October 2026.

## Recommendations
1. Investigate North's revenue decrease by reviewing order volume, product mix, stock availability, and order status.
2. Monitor Electronics product availability and test targeted promotions while considering profitability.
3. Compare Clothing products and regions to identify where focused promotions may help.

## Business Rules and Assumptions
- Revenue includes orders with status `completed` only.
- Revenue is calculated in Indian rupees (INR).
- NULL order amounts must not be treated as confirmed revenue.
- Recommendations are hypotheses to investigate, not proven causes.
- Reported figures should be reconciled with the actual SQL results and cleaned spreadsheet.

## Project Files
- `sql/` — SQL schema, seed data, and analysis queries
- `data/` — cleaned order data and exports
- `results/` — query results and reconciliation evidence
- `docs/dashboard_spec.md` — dashboard design, findings, and recommendations
- `docs/ai_log.md` — AI query verification log

## Dashboard Status
The Tableau Public dashboard contains revenue KPIs and charts for region, category, monthly trend, and region-by-category detail. Confirm the published dashboard URL and access before final submission.

## Final Validation
Before submission, verify that SQL outputs, Excel totals, CSV exports, and Tableau KPIs agree. Include only findings supported by the actual query results.