# Task--3-SQL-BASICS-FILTERING-SORTING-AGGREGATIONS
Step 1 — Table Creation
Column names were defined in SSMS and saved as a new table called table_5. This established the schema for the dataset.
Step 2 — Import CSV
The Superstore CSV file was imported into table_5 using the Import Data wizard with Flat File Source. This populated the table with raw data.
Step 3 — Basic SELECT
A simple query SELECT * FROM table_5; was executed to confirm that rows were loaded. The result displayed the dataset structure and verified the import.
Step 4 — Filtering and Sorting
A query with WHERE category='Technology' ORDER BY sales DESC; was run. This filtered the dataset to Technology products and sorted them by sales in descending order, showing top‑selling items first.
Step 5 — Aggregations
Aggregate functions SUM, AVG, and COUNT were applied with TRY_CAST to handle text fields. This produced grouped totals, averages, and counts by category, confirming numerical analysis worked correctly.
Step 6 — HAVING Clause
A grouped query with HAVING SUM(...) > 100000; was executed to filter categories by total sales. The query ran successfully but returned no rows, meaning no category exceeded the threshold — still valid logic.
Step 7 — BETWEEN and LIKE
Queries using BETWEEN filtered rows within a date range, while LIKE 'A%' searched for customer names starting with “A”. Adjusting column names with brackets (e.g., [customer name]) ensured correct execution.
Step 8 — Export to CSV
Query results were exported by right‑clicking the result grid and choosing Save Results As… → CSV. This created a portable file of the query output.
Step 9 — Views and Procedures
A view was created with CREATE VIEW TechSales AS SELECT * FROM table_5 WHERE category='Technology';. After correcting syntax, the view was successfully queried with SELECT * FROM TechSales;, providing a reusable shortcut for filtered data
