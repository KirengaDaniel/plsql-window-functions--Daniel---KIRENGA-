# plsql-window-functions--Daniel---KIRENGA-
In this presentation, we will demonstrate the use of window functions to address key business questions within a retail sales context. Specifically, we will:
Identify the top-performing products by region,
Analyze customer purchase frequency,
Segment customers for targeted marketing, and
Examine sales data to uncover trends and patterns.

Business Context:
 The case study focuses on a company operating in the retail industry, within the sales department, specializing in the distribution of consumer products.
 
Data Challenge:
 The primary objectives of our analysis are to:
Determine which products achieve the highest sales in each region,
Identify the company’s most frequent and valuable customers, and
Segment customers into groups to support more effective marketing strategies.

STEP 2: Success Criteria

Define exactly 5 measurable goals:

RANK(): This goal is to identify the top five best-selling products within each specific geographical region for every quarter of the year.  The RANK() function is used to assign a rank to each product's sales within its partition (region and quarter), allowing you to filter for the top five.

SUM() OVER(): This goal is used to track the cumulative sales performance over time. It measures the total sales as they accumulate month by month.The SUM() OVER() window function is used to calculate a running total, where the sum of sales for the current month is added to the sum of all preceding months.

LAG()/LEAD(): This goal is to measure the percentage change in sales from one month to the next. It's a key indicator of business momentum and performance. The LAG() or LEAD() functions are used to access the sales value from the previous or next month, allowing for a direct comparison and calculation of the growth rate.

NTILE(4): The NTILE(4) function divides the customer set into four equal partitions, or quartiles. This goal is to categorize customers into four equal groups based on a metric, such as total spending or number of orders.

AVG() OVER(): This goal is to calculate short-term fluctuations in sales data to project/identify longer-term trends.It involves calculating the average sales over a rolling three-month period. 

In our Database we have three tables. Those are : Customers table, Products Table and Transaction table which were used in the implementation of windows function 

<img width="1365" height="767" alt="screenshot 1 for pl" src="https://github.com/user-attachments/assets/cd911a36-24fa-416d-9311-f6e2d8ffb3ee" />
QUERIES:

THE REMAINING QUERIES CAN BE FOUND IN THE NEXT FILE.

RESULT ANALYSIS:

Overall, the objective of these codes is to demonstrate mastery of SQL window functions by applying them to a simple business case (customers, products, and transactions). This provides both operational insights (totals, averages, min/max) and strategic insights (customer segmentation, ranking, and growth).

SOURCES:
->https://www.sqlshack.com/overview-of-sql-rank-functions/
->https://codedamn.com/news/sql/window-functions-row_number-rank-dense_rank-lead-lag-in-sql
->geeksforgeeks.org
->freecodecamp.org
->stratascratch.com
->postgresql.org
->dev.to
->medium.com
->Youtube:“SQL Window Functions in 10 Minutes” – Colt Steele


“All sources were properly cited. Implementations and analysis represent original work. No AI-
generated content was copied without attribution or adaptation.”
