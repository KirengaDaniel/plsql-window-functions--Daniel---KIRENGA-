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

1.RANK(): This goal is to identify the top five best-selling products within each specific geographical region for every quarter of the year.  The RANK() function is used to assign a rank to each product's sales within its partition (region and quarter), allowing you to filter for the top five.

2.SUM() OVER(): This goal is used to track the cumulative sales performance over time. It measures the total sales as they accumulate month by month.The SUM() OVER() window function is used to calculate a running total, where the sum of sales for the current month is added to the sum of all preceding months.

3.LAG()/LEAD(): This goal is to measure the percentage change in sales from one month to the next. It's a key indicator of business momentum and performance. The LAG() or LEAD() functions are used to access the sales value from the previous or next month, allowing for a direct comparison and calculation of the growth rate.

4.NTILE(4): The NTILE(4) function divides the customer set into four equal partitions, or quartiles. This goal is to categorize customers into four equal groups based on a metric, such as total spending or number of orders.

5.AVG() OVER(): This goal is to calculate short-term fluctuations in sales data to project/identify longer-term trends.It involves calculating the average sales over a rolling three-month period. 

In our Database we have three tables. Those are : Customers table, Products Table and Transaction table which were used in the implementation of windows function 

<img width="1365" height="767" alt="screenshot 1 for pl" src="https://github.com/user-attachments/assets/cd911a36-24fa-416d-9311-f6e2d8ffb3ee" />
<img width="1365" height="767" alt="screenshot 2 for pl" src="https://github.com/user-attachments/assets/2fb27187-9577-4b69-b3db-6446cba06ad6" />
<img width="1365" height="767" alt="screenshot 3 q1 for window function insertion" src="https://github.com/user-attachments/assets/19a7e296-1ac0-4788-9b33-bc47f023ba58" /> 
<img width="1365" height="767" alt="screenshot4 q2" src="https://github.com/user-attachments/assets/5f76b172-20c5-438c-8ecf-4c28ba55d8a6" />
<img width="1365" height="767" alt="screenshot4 q2b" src="https://github.com/user-attachments/assets/59042183-97d0-4949-83b6-a7079f4f4aa9" />
<img width="1365" height="767" alt="screenshot4 q2c" src="https://github.com/user-attachments/assets/c17f4931-2844-4c83-9020-1321383f255a" />
<img width="1365" height="767" alt="screenshot4 q4" src="https://github.com/user-attachments/assets/645608d2-edbd-4f4f-b73e-936da8003858" />
<img width="1639" height="1286" alt="er_diagram" src="https://github.com/user-attachments/assets/6d09f660-0edb-4af5-bc19-5f5ad8521e4e" />

QUERIES:

THE REMAINING QUERIES CAN BE FOUND IN THE NEXT FILE.

RESULT ANALYSIS:


Overall, the objective of these codes is to demonstrate mastery of SQL window functions by applying them to a simple business case (customers, products, and transactions). This provides 
both operational insights (totals, averages, min/max) and strategic insights (customer segmentation, ranking, and growth). thanks to windows function we were able to detrmine our most frequent customers, with this information we will be able to create the right advertise and promote commodity that our customer prefer. 

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

