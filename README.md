# plsql_window_functions_-28821-_-GWIRA-
PL/SQL ASSIGNMENT 1
#BUSINESS PROBLEM
##BUSINESS CONTEXT 
An online electronics store named DB ELECTRONICS selling laptops, phones, tablets, and accessories across multiple regions. The sales and marketing department wants better insights into customer behavior and product performance.
##DATA CHALLENGE 
The company struggles to identify top-selling products, track customer purchases over time, and spot patterns that can guide marketing and sales strategies.
##EXPECTED OUTCOME
•	Identify top products per region
•	Analyze customer purchasing frequency
•	Segment customers for targeted marketing
•	Track sales trends
•	Improve decisions on inventory, promotions, and regional strategies

#SCHEMA AND ER DIAGRAM 
##SCHEMA 
Customers(customer_id PK, customer_name, region)
Products(product_id PK, product_name, category, price)
Sales(sale_id PK,customer_id FK,product_id FK,sale_date,quantity,total_amount)
##ER DIAGRAM 
![ER Diagram](Diagrams/ER DIAGRAM.png)

#JOIN QUERIES

## Inner Join

**Purpose:** Retrieve only transactions with valid matching customers and products.

**Diagram:**
![Inner Join Diagram](Diagrams/inner _join.png)

**Business Interpretation:**  
This join ensures we analyze only completed sales with valid data. 
It helps the business focus on real transactions for reporting and decision-making.

## Left Join

**Purpose:** Identify customers who have never made a transaction.

**Diagram:**
![Left Join Diagram](Diagrams/left _join.png)

**Business Interpretation:**  
This join highlights inactive customers. 
The business can target them with marketing campaigns to increase engagement and sales.

## Right Join

**Purpose:** Detect products with no sales activity.

**Diagram:**
![Right Join Diagram](Diagrams/right _join.png)

**Business Interpretation:**  
This join identifies products that aren’t selling. 
Management can decide to promote, discount, or discontinue these items to optimize inventory.

## Full Outer Join

**Purpose:** Compare all customers and products, including unmatched records.

**Diagram:**
![Full Outer Join Diagram](Diagrams/full outer _join.png)

**Business Interpretation:**  
This join provides a complete overview of transactions and gaps in sales. 
It helps identify both inactive customers and unsold products for strategic planning.

## Self Join

**Purpose:** Compare customers within the same region or transactions within the same time period.

**Diagram:**
![Self Join Diagram](Diagrams/self _join.png)

**Business Interpretation:**  
This join reveals patterns or similarities among customers or transactions. 
It supports targeted marketing, regional analysis, and trend identification.







