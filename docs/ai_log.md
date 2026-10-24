# BBD AI Verification Log

## 1. Specification
The task was to calculate revenue by region and identify regions with completed-order revenue greater than ₹80,000. The project defines revenue as the sum of order amounts where the order status is `completed`.

## 2. Execution
The original AI-generated query was reviewed before use. It referenced a `sales` table and columns named `region_name` and `total_sales`. These names do not match the project schema. It also used `SUM(total_sales)` in the `WHERE` clause.

## 3. Inspection
Four defects were identified:
1. The table `sales` does not exist in the project schema.
2. The columns `region_name` and `total_sales` do not match the project schema.
3. Aggregate functions such as `SUM()` cannot be used directly in `WHERE`; use `HAVING` to filter grouped results.
4. The claim that North's revenue grew by 38% month over month was unsupported and conflicts with the verified September-to-October decrease of 22.8%.

## 4. Verification
The corrected query must use the actual orders and customer/region schema, count only completed-order revenue, group the results by region, and filter groups using `HAVING SUM(amount) > 80000`. The expected results are North: ₹119,300 and South: ₹82,500. These figures must be checked against the executed SQL output before submission.

## 5. Decision
Reject the original query because it uses invalid table and column names, places an aggregate in `WHERE`, and supports an inaccurate business claim. Accept the corrected query only after its executed results match the project data and the revenue definition.

## Evidence and Limitations
- Revenue includes completed orders only.
- North's revenue decreased by 22.8% from September to October 2026.
- The verification should be supported by the saved SQL query and its actual result output.
- AI-generated claims must be checked against the dataset before being shared with a manager.