Spreadsheet Cleaning and Reconciliation Notes

1. Workbook and Tools

- Tool used: Microsoft Excel
- Working workbook: BBD_working.xlsx
- Cleaned data export: orders_clean.csv
- Source worksheet: orders
- Product lookup worksheet: products
- Final cleaned worksheet: completed_orders

2. Cleaning and Lookup Formulas

- Clean first name: "=PROPER(TRIM(C2))"
- Clean last name: "=PROPER(TRIM(D2))"
- Product category: "=VLOOKUP(G2,products!$A$2:$C$10,2,FALSE)"
- Unit price: "=XLOOKUP(G2,products!$A$2:$A$10,products!$C$2:$C$10,"UNKNOWN_ITEM")"
- Calculated revenue: "=N2*H2"

The original order amount was retained for reconciliation. Revenue calculations use cell references rather than hard-coded prices.

3. Summary Statistics

Metric| Result
Completed orders| 63
Total amount / revenue (INR)| 346200
Average amount (INR)| 5495.24
Minimum amount (INR)| 1100
Maximum amount (INR)| 15600

4. PivotTable Results

PivotTable 1: Revenue by Category and Region

- Rows: category
- Columns: region
- Values: Sum of amount
- Grand Total: ₹346,200

PivotTable 2: Revenue by Month

- Rows: order_month
- Values: Sum of amount and Count of order_id
- Grand Total for Sum of amount: ₹346,200

5. Reconciliation

The cleaned CSV contains 63 completed orders. The sum of the amount column is ₹346,200, matching the SQL q05 result of 63 completed orders and ₹346,200 total revenue.

6. Data Quality and Validation

- Three order records had missing amounts in the source dataset; these should be checked against the SQL q02 results.
- Four customers in the original customer table had no orders.
- Product lookups should be checked for any "UNKNOWN_ITEM" values.
- Check for duplicate order IDs and unusually high order amounts before final submission.
- The original amount field was retained separately from revenue_calc to support reconciliation.

7. Export

The final export is orders_clean.csv with 13 columns and 63 completed-order records. The order_month field should remain text, for example "2026-09".