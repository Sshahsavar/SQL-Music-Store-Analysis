# Digital Music Store Data Analysis (SQL)

## Project Overview
This project involves a comprehensive SQL-based data analysis of a simulated digital music store (based on the Chinook Database). The goal of this project is to extract actionable business insights regarding customer purchasing behavior, regional sales performance, product inventory, and employee workload.

## Skills & SQL Techniques Demonstrated
- **Advanced Joins:** `INNER JOIN`, `LEFT JOIN`, `NOT IN` handling missing/incomplete data.
- **Window Functions:** `ROW_NUMBER()`, `LAG()`, and `OVER(PARTITION BY...)` for cohort and time-between-purchase analysis.
- **Common Table Expressions (CTEs) & Subqueries:** Structuring complex logic for Pareto analysis (80/20 rule) and top-tier demographics.
- **Conditional Logic:** `CASE WHEN` for customer segmentation and product categorization.
- **Aggregations & Date Manipulation:** `GROUP BY`, cumulative sums, and `JULIANDAY`/`strftime` for year-over-year (YoY) trends.

## Key Business Questions Answered
1. **Customer Analytics:** 
   - Calculated Customer Lifetime Value (CLV) and cumulative running totals.
   - Identified first vs. latest purchase dates and amounts to track retention.
   - Calculated the average time (in days) between a customer's first and second purchase.
   - Segmented customers into 'Major', 'Standard', and 'Low' purchasing tiers.
2. **Sales & Geographic Trends:** 
   - Ranked top donors/customers globally and regionally.
   - Compared North American revenue versus the rest of the world.
   - Calculated YoY revenue growth and year-to-year customer retention (2009 vs 2010).
3. **Employee Performance:** 
   - Categorized support representatives based on workload capacity.
   - Identified high-performing staff managing over $800 in total sales.
4. **Product Insights:** 
   - Categorized tracks by length (Short, Medium, Long) to correlate with unit price.
   - Identified zero-revenue tracks and genres that have never been purchased.

## How to Run
The queries in this repository are written in **SQLite**. They can be run against the standard Chinook SQLite database using any compatible SQL client (e.g., DBeaver, DB Browser for SQLite, or an online SQLite compiler).
