# Pizza-Sales---SQL-Project
This project is a comprehensive Data Analysis for a real-world pizza restaurant chain. I utilised MySQL to analyse sales, orders, and pricing data to derive actionable insights that can optimise operations, inventory, and marketing strategies


## 🔑 Key SQL Concepts Demonstrated**
- **Data Joins:** Used `LEFT JOIN` and `INNER JOIN` to connect `orders`, `order_details`, and `pizzas` tables to calculate metrics requiring cross-table data (e.g., total quantity of each pizza category ordered ).
- **Aggregation:** Extensive use of `GROUP BY`, `SUM()`, `COUNT()`, and `AVG()` for calculating total orders and average pizzas per day.
- **Window Functions:** Implemented `SUM()` `OVER` `(ORDER BY date)` to calculate the *cumulative (running total) revenue* generated over time. 
- **Common Table Expressions (CTEs):** Used *CTEs* to modularise complex queries, such as the *calculation for the percentage contribution of each pizza type to total revenue* and determining the top 3 most ordered pizza types based on revenue for each category  using `RANK()` or `ROW_NUMBER()` partitioned by category.
- **Date/Time Functions:** Utilised functions like `HOUR()` or `EXTRACT(HOUR FROM column)` to determine the distribution of orders by hour of the day.
- **Subqueries:** Employed **nested queries** to filter and aggregate data efficiently before joining or final reporting.

 ## 📊 Key Analytical Questions Answered 
**1. Basic Metrics (Foundational Aggregation)**
  - Retrieved the **Total Number of Orders Placed.**
  - Calculated the **Total Revenue generated from all pizza sales.**
  - Identified the **Highest-Priced Pizza.**
  - Determined the **Most Common Pizza Size ordered, crucial for inventory planning.**
  - Listed the **Top 5 Most Ordered Pizza Types by quantity.**

**2. Intermediate Analysis (Complex Joins & Aggregation)**
  - Calculated the **Total Quantity of Each Pizza Category ordered.**
  - Analyzed the **Distribution of Orders by Hour of the Day, pinpointing peak hours for staffing.**
  - Calculated the **Average Number of Pizzas** Ordered Per Day across the dataset.
  - Identified the **Top 3 Most Ordered Pizza Types** based on Revenue.

**3. Advanced Insights (Analytical & Comparative Functions)**
  - Calculated the **Percentage Contribution of Each Pizza Category to Total Revenue**, a key financial metric.
  - Analyzed the **Cumulative Revenue Generated Over Time** using a window function for trend tracking.
  - Determined the **Top 3 Most Ordered Pizza Types based on Revenue for Each Pizza Category** using partitioned ranking.
