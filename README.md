# 🛒 Target Brazil — Case Study

## 📌 Project Overview
This project analyzes **Target’s operations in Brazil** using order-level, customer, seller, payment, review, and geolocation data from 2016–2018 (100k+ orders).  
The goal was to derive **business insights using SQL queries**

---

## 🎯 Problem Statement
Target wants to better understand:
- Is there a **growing trend** in the no. of orders placed over the past years?
- Can we see some kind of **monthly seasonality** in terms of the no. of orders being placed?
- During **what time of the day**, do the Brazilian customers mostly place their orders? (Dawn, Morning, Afternoon or Night)
     0-6 hrs   : Dawn
     7-12 hrs  : Mornings
     13-18 hrs : Afternoon
     19-23 hrs : Night
- How efficient are their **order processing and deliveries**?  
- Which **products, sellers, and regions** drive revenue or underperform?  
- How do **freight charges and payment methods** impact order values?   


## 📂 Dataset
The dataset consists of **8 CSVs**:  
`customers.csv`, `sellers.csv`, `orders.csv`, `order_items.csv`, `products.csv`, `payments.csv`, `reviews.csv`, `geolocation.csv`.

Each table was loaded into SQL and joined using **keys such as `order_id`, `customer_id`, `product_id`, `seller_id`, and zip code prefixes.**

---

## 🔎 Approach
1. **Data Preparation**
   - Imported all CSVs into SQL tables.
   - Validated relationships across tables.
   - Standardized date formats for order timelines.

2. **SQL Analysis**
   - Customer behavior: revenue by state/city.  
   - Seller performance: average delivery times, on-time vs delayed orders.  
   - Monthly seasonality: Month on month no. of orders placed in each state.
   - Operational metrics: freight cost share of revenue, payment type usage.  
 

3. **KPIs Calculated**
   - Average shipping time vs estimated delivery date.  
   - % of late deliveries.  
   - Average Order Value (AOV) by payment type & installments.  
   - Freight as % of product price.  
---

# Project Report 
You can access the complete project report here - [Report](https://github.com/kriti2011/Target-Case-Study/blob/main/Target_Business_Case_SQL_Kriti_Pahuja.pdf)

## ✅ Key Insights

- There is a **growing trend** in the number of orders over the past years.
- Highest number of orders have been placed in the afternoon (possibly because people take lunch breaks during work) and after 7 PM in the evening(when people are free from their work)
- **Delivery delays** strongly impacted number of orders. 
- **Top regions** (São Paulo) accounted for majority of sales but also had the **highest congestion-related delays**.  
- Certain **sellers consistently underperformed** in delivery timelines, dragging overall satisfaction.
- **Payment Method** is also a major factor, as we can see highest number or orders being placed from credit card.
- **Monthly seasonality** has also affected the number of orders being placed. Highest number of orders have been placed during August,May and July  Month, means, during mid-winter in Brazil(July,August) and also during cultural holidays (like Mother’s Day widely celebrated in Brazil in May). 

## 💡 Recommendations

- Improve **logistics partnerships** by launching more stores or warehouses and partnering with more local delivery companies in high-delay regions.  
- Introduce **free/discounted shipping thresholds** to optimize freight-to-price ratio.  
- **Discounts on credit cards** because it is the mostly used payment method especially in the months of May,July and August. .  
- Run digital ads and push notifications between 1–3 PM (lunch) and 7–10 PM (family & shopping time). 
- Encourage installment-based payments for **high-value categories** like credit card with no-cost EMI options. 
- Special products,discount and offers during festival months(like **Mother's Day in May**) and **New Year & Christmas Preparations** during November-January.

## 🛠️ Tech Stack
- **SQL (BigQuery)** for all analysis  
- Joins, aggregations, window functions, date/time calculations, subqueries


