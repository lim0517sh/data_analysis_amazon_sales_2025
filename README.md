# data_analysis_amazon_sales_2025
https://www.kaggle.com/datasets/zahidmughal2343/amazon-sales-2025/data

# Context of Data
- Order ID - Unique identifier for each order (e.g., ORD0001)
- Date - Date of the order
- Product - Name of the product purchased
- Category - Product category (Electronics, Clothing, Home Appliances, etc.)
- Price - Price of a single unit of the product
- Quantity - Number of units purchased in the order
- Total Sales - Total revenue from the order (Price × Quantity)
- Customer Name - Name of the customer
- Customer Location - City where the customer is based
- Payment Method - Mode of payment (Credit Card, Debit Card, PayPal, etc.)
- Status - Order status (Completed, Pending, or Cancelled)

# Project Motivation
In this project, I focused on enabling stakeholders to quickly and accurately understand monthly performance. At the same time, I added conditional components them  so they can easily check yearly and quarterly performance as well.
At first, I contained commerce major and general metrics in the dashboard such as sales volume, order volume, and AOV. In order to deliver not only static information, but also time series information, I added MoM growth to the sales volume and sales volume metrics.

Initially, I included key commerce and general metrics in the dashboard, such as sales volume, order volume, and average order value (AOV). To provide not only static information but also time series insights, I added month-over-month (MoM) growth rates for both sales volume and order volume.

The second feature is a comparison between all orders and completed orders. During my analysis, I found that the proportion of completed orders was relatively low compared to total orders. To help stakeholders view performance from multiple perspectives, I designed the dashboard with two legends: one for all orders and one for completed orders.
Finally, I used various types of charts to help users better understand the data.

# Data Cleansing
Even though I went over the dataset based on the CLEAN framework suggested by Christine Jiang(1), the founder of theanalyticsaccelerator.com, I only corrected the Date column. The date formats were inconsistent (some entries were in dd/mm/yy, others in yy-mm-dd), so I added a column named "date_cleaned" with all dates standardized to the "yy/mm/dd" format.
Additionally, I added three columns: two for deriving completed orders data, and one for extracting the month.

# Results
**Low completion rate** : 
The sales showed a low completion rate. While the total sales were $243,845 in 2025, the completed sales were $88,530. The order volume showed almost same result. Order volume displayed a similar trend: out of 250 total orders in 2025, only 88 were completed. This means about one-third of orders were completed, indicating a need for improvement(2).

**Volatile performance** : 
The performance varied rapidly month by month. In February, sales volume and order volume soared by 3,560% and 1,900%, respectively. However, in April, these metrics decreased by 83.8% and 93.8%.

# Reference
(1) https://www.youtube.com/watch?v=iYEw8L3Un4c
(2) https://www.persado.com/articles/checkout-completion-rate/#:~:text=The%20average%20checkout%20completion%20rate,Performance%20monitoring
