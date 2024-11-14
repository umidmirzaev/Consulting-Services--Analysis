# Consulting-Services-Analysis

## Business Objectives & User Stories

This project involved creating a Consulting Services Dashboard to provide an at-a-glance view of key metrics relevant to consulting sales performance. The dashboard was developed to address specific business needs identified by the sales and marketing team, focusing on tracking revenue, sales dynamics, customer engagement, and product performance. Below are the objectives and user requirements that guided the dashboard design.

### Business Objectives:
1. **Monitor Sales Performance**
Provide a clear overview of sales figures, including total revenue, number of sales, average revenue per sale, and average purchase frequency. The goal is to allow stakeholders to track overall sales performance and identify trends over time.
   
2. **Product Performance Analysis**
Highlight which consulting products are generating the highest revenue and most sales. This analysis will help the business determine which services are most profitable and where there may be opportunities for increased marketing efforts.
   
3. **Customer Engagement Tracking**
Track customer interaction metrics, such as the number of received, opened, and clicked emails, to understand engagement levels. This helps the marketing team evaluate the effectiveness of email campaigns and determine which products are receiving the most customer interest.

4. **Sales Dynamics Visualization**
Provide a monthly trend of sales and revenue to help the business understand seasonality and patterns in consulting services demand. This enables better forecasting and resource allocation.

### User Requirements:

| #  | Role                         | Request/Demand                                             | User Value                                                   | Acceptance Criteria                                            |
|----|-------------------------------|------------------------------------------------------------|--------------------------------------------------------------|----------------------------------------------------------------|
| 1  | **Sales Manager**             | See a summary of total revenue and number of sales         | Monitor overall sales performance                            | A high-level view of total revenue, number of sales, and key metrics |
| 2  | **Marketing Analyst**         | Analyze the performance of each consulting product         | Identify which services are most popular and profitable      | A breakdown by product showing sales and revenue per service     |
| 3  | **Sales Representative**      | Track customer engagement with our email campaigns         | Understand customer responses to marketing efforts           | Metrics showing number of emails received, opened, clicked, and their relation to sales |
| 4  | **Product Manager**           | Compare monthly sales trends over time                     | Identify seasonal demand patterns and forecast future sales  | A dynamic line chart displaying monthly trends of sales and revenue |
| 5  | **Executive**                 | View a breakdown of product sales by percentage            | Assess product lines contributing most to overall sales      | A visual chart showing percentage breakdown of product sales |


## Data Transformation

In this project, I utilized Power BI's DAX (Data Analysis Expressions) to transform and calculate key performance metrics for the Consulting Services Dashboard. These DAX measures enabled tracking of essential metrics like revenue, sales volume, user engagement, and other KPIs to provide a comprehensive view of consulting service performance.

### Key DAX Measures:

1. **Average Purchase Frequency**  
   This measure calculates the average number of purchases per user, helping identify customer purchasing behavior over time.

2. **Average Revenue**  
   Calculated to understand the average revenue generated per transaction, allowing stakeholders to gauge the typical transaction value.

3. **Average Revenue per User (ARPU)**  
   This measure determines the average revenue generated per unique user, providing insights into customer value.

4. **Click Rate (CR)**  
   A metric that calculates the click-through rate of marketing emails, helping assess user engagement and interest in specific services.

5. **Individual Open Rate (IOR)**  
   Tracks the percentage of users who opened an email, which is essential for understanding the reach and effectiveness of email campaigns.

6. **No. of Sales**  
   The total number of sales transactions, representing the volume of consulting services sold over the specified period.

7. **No. of Unique Users**  
   Counts the unique users who made purchases, useful for understanding the customer base size and engagement.

8. **Open Rate (OR)**  
   A measure of the percentage of emails opened out of the total sent, useful for evaluating email campaign effectiveness.

9. **Total Revenue**  
   Summarizes the revenue generated from all sales, providing a high-level view of the business's financial performance.

10. **Unique Openers**  
    Calculates the number of unique users who opened an email, allowing the marketing team to understand campaign reach among distinct individuals.

### Data Model Structure

**Consulting Services Analysis - Data Model**   
![DataModel](https://github.com/umidmirzaev/Consulting-Services--Analysis/blob/main/semantic.png)

The data model connects multiple tables to enable analysis across customer engagement and sales. Here is an overview of the tables and their roles in the model:

- **CustomerEmail**  
  Contains email interaction data such as emails opened, emails received, and clicks. This table is essential for tracking customer engagement metrics.

- **CustomerSales**  
  Holds sales transaction data, including customer ID, product, and transaction value. It provides the core data for revenue and sales metrics.

- **DimDate**  
  A date dimension table that allows filtering and analyzing data over different time periods, facilitating trend analysis.

- **DimId**  
  Serves as an identifier table, allowing relationships between different entities in the model.

- **Measure Table**  
  Contains DAX measures created to calculate the essential KPIs and performance metrics for the dashboard.

This data model and the DAX measures empower the dashboard to deliver valuable insights into consulting sales performance, customer engagement, and product profitability, all in an interactive and visually compelling format.


## Dashboard Overview:
The final dashboard includes:
- **High-Level Metrics**: Displaying total revenue, average revenue per sale, average revenue per user, and purchase frequency.
- **Sales & Revenue Dynamics**: A monthly trend chart of sales and revenue to track growth and patterns over the year.
- **Product Performance**: A detailed view of product performance in terms of sales volume and revenue.
- **Customer Interaction Analysis**: A table summarizing customer email engagement metrics and corresponding sales data.
- **Product Sales Breakdown**: A pie chart showing the percentage of sales per product category for quick insights into product contribution.

**Consulting Services Analysis - Overview Page**
![Overview Page](https://github.com/umidmirzaev/Consulting-Services--Analysis/blob/main/Overview.png)
