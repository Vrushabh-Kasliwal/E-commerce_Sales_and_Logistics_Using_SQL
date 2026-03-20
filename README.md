# E-commerce Sales & Logistics SQL Analysis

## 📌 Overview  
This project analyzes **100K+ e-commerce orders (2016–2018)** to uncover:  
- Growth trends  
- Customer behavior  
- Payment & delivery performance  
- Logistics inefficiencies  

## 📌 Context  
This case study focuses on the operations of a **leading e-commerce retailer** in Brazil, analyzing **100,000 orders** placed between **2016 and 2018**.  

The dataset provides insights into various business aspects, including:  
✔ **Order processing & status**  
✔ **Pricing strategies**  
✔ **Payment & shipping efficiency**  
✔ **Customer demographics**  
✔ **Product attributes & customer reviews**  

By analyzing this dataset, we can understand **order trends, revenue patterns, customer preferences, and logistics performance**.  

## 📂 Dataset Information  
- The dataset includes **orders, customers, payments, and delivery details**.  
- Time period: **2016–2018**  
- Contains information on **order status, pricing, shipping, customer demographics, and reviews**.  

## 🔍 Key Insights  
✔ **E-commerce orders grew significantly**, except for a decline in Sep–Oct 2018.  
✔ **Sales peak in January, March, and August**.  
✔ **Credit cards are the most preferred payment method**.  
✔ **Some states face delivery delays of 27+ days**, affecting customer experience.  

## 🛠 SQL Queries Used  
- **Exploratory Data Analysis (EDA)**: Data types, time range, customer locations  
- **Growth Trends**: Monthly trends, seasonality  
- **Delivery Performance**: Time to delivery, freight cost  
- **Payment Analysis**: Popular payment methods, installment trends  

## 📊 Sample SQL Query  
```sql
SELECT customer_state, COUNT(*) AS customer_count
FROM ecom_customers
GROUP BY customer_state
ORDER BY customer_count DESC
LIMIT 5;
