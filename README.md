# plsql_window_functions_-28821-_-GWIRA-
PL/SQL ASSIGNMENT 1

# Business Problem

## Business Context
DB ELECTRONICS is an online electronics store selling laptops, phones, tablets, and accessories across multiple regions. The sales and marketing department wants better insights into customer behavior and product performance.

## Data Challenge
The company struggles to identify top-selling products, track customer purchases over time, and spot patterns that can guide marketing and sales strategies.

## Expected Outcome
- Identify top products per region  
- Analyze customer purchasing frequency  
- Segment customers for targeted marketing  
- Track sales trends  
- Improve decisions on inventory, promotions, and regional strategies  

# Schema and ER Diagram

## Schema
**Customers**(`customer_id` PK, `customer_name`, `region`)  
**Products**(`product_id` PK, `product_name`, `category`, `price`)  
**Sales**(`sale_id` PK, `customer_id` FK, `product_id` FK, `sale_date`, `quantity`, `total_amount`)  

## ER Diagram
![ER Diagram](Diagrams/ER DIAGRAM.png)

# Join Queries

## Inner Join

**Purpose:** Retrieve only transactions with valid matching customers and products.

**Screenshot:**
![Inner Join Diagram](Diagrams/inner _join.png)

**Business Interpretation:**  
This join ensures we analyze only completed sales with valid data. 
It helps the business focus on real transactions for reporting and decision-making.

## Left Join

**Purpose:** Identify customers who have never made a transaction.

**Screenshot:**
![Left Join Diagram](Diagrams/left _join.png)

**Business Interpretation:**  
This join highlights inactive customers. 
The business can target them with marketing campaigns to increase engagement and sales.

## Right Join

**Purpose:** Detect products with no sales activity.

**Screenshot:**
![Right Join Diagram](Diagrams/right _join.png)

**Business Interpretation:**  
This join identifies products that aren’t selling. 
Management can decide to promote, discount, or discontinue these items to optimize inventory.

## Full Outer Join

**Purpose:** Compare all customers and products, including unmatched records.

**Screenshot:**
![Full Outer Join Diagram](Diagrams/full outer _join.png)

**Business Interpretation:**  
This join provides a complete overview of transactions and gaps in sales. 
It helps identify both inactive customers and unsold products for strategic planning.

## Self Join

**Purpose:** Compare customers within the same region or transactions within the same time period.

**Screenshot:**
![Self Join Diagram](Diagrams/self _join.png)

**Business Interpretation:**  
This join reveals patterns or similarities among customers or transactions. 
It supports targeted marketing, regional analysis, and trend identification.

## WINDOW FUNCTIONS

## Ranking Functions

**Purpose:** Identify top-performing customers and products based on revenue.

**Screenshots:**
![Top Customers by Revenue](Diagrams/top customers by revenue.png)
![Top Products by Revenue](Screenshots/top products by revenue.png)

**Business Interpretation:**  
Ranking functions help the business quickly identify high-value customers and best-selling products. 
This supports targeted marketing, loyalty rewards, and inventory prioritization for maximum revenue.

## Aggregate Window Functions

**Purpose:** Calculate cumulative metrics and trends over time.

**Screenshots:**
![Running Total Sales by Date](Diagrams/running total of sales by date .png)
![Three-Month Moving Average for Trends](Diagrams/three month moving average using range for trends.png)

**Business Interpretation:**  
Aggregate window functions provide insights into cumulative performance and sales trends. 
They help management forecast revenue, track growth, and make informed operational decisions.

## Navigation Functions

**Purpose:** Compare metrics across periods to measure growth or decline.

**Screenshot:**
![Period-to-Period Comparison](Diagrams/navigation function.png)

**Business Interpretation:**  
Navigation functions allow the business to analyze period-to-period changes. 
They help identify trends, seasonality, and growth patterns, enabling better planning and strategy adjustments.

## Distribution Functions

**Purpose:** Segment customers based on revenue or other performance metrics.

**Screenshot:**
![Customer Segmentation](Diagram/distribution function.png)

**Business Interpretation:**  
Distribution functions categorize customers into meaningful segments. 
This supports targeted marketing, personalized promotions, and resource allocation to improve retention and profitability.

## Key Insights

This SQL project demonstrates how to effectively manage and analyze sales data using relational database techniques. By implementing various joins, we identified valid transactions, inactive customers, unsold products, and gaps in sales. Window functions provided deeper analytical insights, such as ranking top customers and products, tracking running totals and trends, comparing period-to-period growth, and segmenting customers for targeted strategies. Overall, this work highlights the importance of structured data, precise queries, and actionable analysis in driving business decisions and improving revenue management.

## Result Analysis

**Descriptive:**  
The analysis revealed that most transactions involve a subset of active customers and popular products, while some customers have never made purchases and certain products remain unsold. Ranking functions highlighted the top-performing customers and products by revenue, while aggregate window functions tracked cumulative sales and trends over time. Navigation functions allowed period-to-period comparisons, and distribution functions segmented customers into meaningful groups.

**Diagnostic:**  
Inactive customers and unsold products are likely due to lack of engagement or low demand, as shown by left and right joins. Sales trends and period comparisons indicate seasonal patterns and fluctuations in revenue, explaining why some products outperform others. Customer segmentation suggests a concentration of revenue among a small group of high-value clients.

**Prescriptive:**  
To optimize business performance, management should target inactive customers with promotions and loyalty programs, consider marketing or discontinuing unsold products, and focus inventory and sales strategies on high-performing products. Trend insights should guide operational and financial planning, while segmentation can inform personalized marketing and strategic customer relationship management.

## Integrity Statement

I hereby declare that this SQL assignment and all associated work, including queries, diagrams, screenshots, and analyses, are my own original efforts. I have not engaged in plagiarism, and all sources used for reference have been properly cited. I take full responsibility for the authenticity and accuracy of this work.

## References

1. Oracle Documentation. *SQL Language Reference*. Oracle Corporation. [https://docs.oracle.com/en/database/oracle/oracle-database/](https://docs.oracle.com/en/database/oracle/oracle-database/)  
2. PostgreSQL Global Development Group. *PostgreSQL: Documentation*. [https://www.postgresql.org/docs/](https://www.postgresql.org/docs/)  
3. W3Schools. *SQL Tutorial*. [https://www.w3schools.com/sql/](https://www.w3schools.com/sql/)  
4. Mode Analytics. *SQL Window Functions Guide*. [https://mode.com/sql-tutorial/sql-window-functions/](https://mode.com/sql-tutorial/sql-window-functions/)  
5. DataCamp. *Introduction to SQL Joins*. [https://www.datacamp.com/tutorial/sql-joins](https://www.datacamp.com/tutorial/sql-joins/)  
6. GeeksforGeeks. *SQL Joins and Window Functions*. [https://www.geeksforgeeks.org/sql-joins/](https://www.geeksforgeeks.org/sql-joins/)  
7. Stack Overflow. *SQL Queries and Best Practices*. [https://stackoverflow.com/questions/tagged/sql](https://stackoverflow.com/questions/tagged/sql)  
8. “Learning SQL” by Alan Beaulieu, 3rd Edition, O’Reilly Media, 2020.














