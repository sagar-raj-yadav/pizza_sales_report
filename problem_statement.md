
## 1.PROBLEM STATEMENT:

We are required to analyze key performance indicators (KPIs) for pizza sales data to gain insights into the business performance. Specifically, we want to calculate the following metrics:

i.Total Revenue: The sum of the total price of all pizza orders.

ii.Average Order Value: The average amount spent per order, calculated by dividing the total revenue by the total number of orders. (ek order pe average kitna paisa kharch hota hai.)

Average Order Value= Total Number of Orders/Total Revenue

iii.Total Pizzas Sold: The sum of the quantities of all pizzas sold.

iv.Total Orders: The total number of orders placed.

v.Average Pizzas Per Order: The average number of pizzas sold per order.

Average Pizzas Per Order= Total Orders/Total Pizzas Sold
​
 
Note:- KPI ->Yeh ek measurable value hota hai jo kisi organization ya business ki performance ko track karta hai. KPIs help karte hain yeh samajhne mein ki koi business ya team apne objectives ko kitna effectively achieve kar raha hai.

## 2. CHARTS REQUIREMENT:
i.Daily trend fro total orders->create a bar chart that displays the trend of total orders over a specific time period.This chart helps use to identify any patterns in order volumes on a daily basis.

ii.hourly trend of total orders->create a line chart that shows the hourly of total orders throughout the day.This chart will help us to identify peak hours of high order activity.

iii.percentage of sales by pizze category->create a pie chart that shows the distribution of sales across different pizza categories .This chart wil provide insights into the popularity of various pizza categories and their contribution to overall sales.

iv.pecentage of sales by pizza size->generate a pie chart that represents the percentage of sales atrributed to different pizza sizes.This chart will help us to understand customer preferences for pizza and their impact on sales.

v.Total Pizzas Sold by Pizza Category:
Create a funnel chart that presents the total number of pizzas sold for each pizza category. This chart will allow us to compare the sales performance of different pizza categories.

Vi.Top 5 Best Sellers by Total Pizzas Sold:
Create a bar chart highlighting the top 5 best-selling pizzas based on the fotal number of pizzas sold. This chart will help us identify the most popular pizza options.

7.Bottom 5 Worst Sellers by Total Pizzas Sold:
Create a bar chart showcasing the bottom 5 worst-selling pizzas based on the total number of pizzas sold. This chart will enable us to identify underperforming or less popular pizza opfions.

# software used
MS EXCEL AND MS SQL SERVER


### PIZZA SALES SQL QUERY
# KPI's

i.Total Revenue: 
SELECT SUM(total_price) AS total_revenue
FROM pizza_sales;

ii.Average Order Value:
SELECT SUM(total_price)/COUNT(DISTINCT order_id) AS Average_Order_Value from pizza_sales

iii.Total Pizzas Sold:
SELECT SUM(quantity) AS Total_pizza_sold from pizza_sales 

iv.Total Orders:
SELECT COUNT(DISTINCT order_id) AS Total_orders from pizza_sales 


v.Average Pizzas Per Order: 