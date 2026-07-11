# 📊 Quick-Commerce Analytics

An end-to-end retail analytics project that leverages **Python** and **Power BI** to analyze customer purchasing behavior, sales trends, reorder patterns, and product associations using the **Instacart Online Grocery Shopping Dataset**. The project transforms raw transactional data into interactive dashboards and actionable business insights to support data-driven decision-making.

---

## 📖 Project Overview

Retail businesses generate millions of customer transactions every day. Understanding these transactions helps organizations improve inventory management, optimize marketing campaigns, and enhance customer satisfaction.

This project analyzes real-world retail transaction data to identify purchasing patterns, customer ordering behavior, reorder trends, and product associations. Python was used for data preprocessing, dataset merging, and Market Basket Analysis using the Apriori algorithm, while Power BI was used to develop interactive dashboards for sales, customer, and product association analysis.

---

## 🎯 Project Objectives

This project aims to answer the following business questions:

- Which products are ordered most frequently?
- Which departments contribute the highest number of orders?
- During which hours and days do customers place the most orders?
- How are customer ordering frequencies distributed?
- What is the average time between customer orders?
- Which products are frequently purchased together?
- How can these insights support product recommendations, cross-selling, and inventory planning?

---

## 📂 Dataset

**Dataset:** Instacart Online Grocery Shopping Dataset

**Source:** Kaggle

The dataset contains anonymized customer order history collected from Instacart, including customer orders, products, aisles, and departments. It provides a realistic retail environment for performing customer analytics and product recommendation analysis.

### Files Used

* orders.csv
* order_products__prior.csv
* products.csv
* aisles.csv
* departments.csv

---

## 🛠️ Technologies Used

### Programming

* Python

### Libraries

* Pandas
* NumPy
* mlxtend (Apriori Algorithm)

### Visualization

* Microsoft Power BI
* DAX

### Development Environment

* Visual Studio Code

---

## 🔄 Project Workflow

The project follows an end-to-end analytics pipeline, transforming raw retail transaction data into meaningful business insights through data preprocessing, market basket analysis, and interactive dashboards.

```text
          Kaggle Instacart Dataset
                    │
                    ▼
        Data Loading & Preprocessing
                 (Python)
                    │
                    ▼
          Dataset Merging & Cleaning
                    │
                    ▼
        Exploratory Data Analysis
                    │
         ┌──────────┴──────────┐
         ▼                     ▼
 Power BI Dashboards    Market Basket Analysis
                               (Apriori Algorithm)
         ▼                     ▼
 Sales & Customer      Association Rules
     Analytics                │
         └──────────┬──────────┘
                    ▼
     Business Insights & Decision Support
```
---
### 📈 Page 1 – Sales Analytics

The Sales Analytics dashboard provides an overview of overall sales performance, product demand, customer activity, and ordering trends. It enables stakeholders to monitor business performance through key performance indicators and interactive visualizations.

**Visuals Included**
- KPI Cards (Total Orders, Total Products, Total Customers, Reorder Rate)
- Top 10 Best-Selling Products
- Product Distribution by Department
- Peak Ordering Hours
- Weekly Ordering Pattern
- Top 10 Reordered Products

> 📷 **Sales Analytics Dashboard**
>
><p align="center">
  <img width="700" alt="Sales Analytics Dashboard" src="https://github.com/user-attachments/assets/e4922013-7fbb-4dd6-a23a-33d4fc0973a6" />
</p>

### 👥 Page 2 – Customer Analytics

The **Customer Analytics** dashboard focuses on understanding customer purchasing behavior, ordering frequency, and reorder patterns. It provides valuable insights into how customers interact with the platform, helping businesses improve customer retention, demand forecasting, and personalized marketing strategies.

**Visuals Included**
- KPI Cards (Total Customers, Average Days Between Orders)
- Customer Ordering Behavior (Scatter Plot)
- Distribution of Orders per Customer (Histogram)
- Reorder Interval Distribution (Histogram)

>📷 **Customer Analytics Dashboard**
>
><p align="center">
  <img width="700" alt="Customer Analytics Dashboard" src="https://github.com/user-attachments/assets/ccde8844-a1ee-4f15-adef-7b3317450c6e" />
</p>

### 🛒 Page 3 – Market Basket Analysis

The **Market Basket Analysis** dashboard presents the results of association rule mining using the **Apriori Algorithm**. It helps identify products that are frequently purchased together by evaluating association metrics such as **support**, **confidence**, and **lift**. These insights can be used to improve product recommendations, cross-selling strategies, promotional campaigns, and inventory planning.

**Visuals Included**
- KPI Cards (Total Association Rules, Average Lift, Average Confidence)
- Top 10 Products Bought Together (Association Rules Table)
- Support vs Confidence Scatter Plot

>📷 **Market Basket Analysis Dashboard**
>
><p align="center">
  <img width="700" alt="Market Basket Analysis Dashboard" src="https://github.com/user-attachments/assets/6ca36d65-3336-46f7-aa43-3d7c91c539f6" />
</p>

---

## 🔍 Key Business Insights

### 📈 Sales Analytics

- The dataset contains **3.42 million orders** placed by approximately **206.21K customers**, covering nearly **35K unique products**.
- The overall **reorder rate is 59%**, indicating that more than half of all purchases are repeat orders, reflecting strong customer loyalty.
- **Banana** is the highest-selling product with approximately **14.5K orders**, followed by **Bag of Organic Bananas (11.7K)** and **Organic Strawberries (8.1K)**.
- Customer activity peaks between **9 AM and 4 PM**, with the highest order volume occurring around **10–11 AM**, suggesting this is the busiest shopping window.
- Weekly ordering trends show the highest number of orders on **Sunday (~0.60M)**, followed closely by **Monday (~0.59M)**, while **Thursday records the lowest order volume (~0.43M)**.
- Fresh produce dominates customer purchases, with products such as bananas, avocados, lemons, strawberries, and raspberries consistently appearing among the top-selling items.

### 👥 Customer Analytics

- The platform serves approximately **206.21K customers**, with an **average interval of 11.13 days** between consecutive orders.
- The **Orders per Customer** distribution shows a sharp concentration of customers with **low order frequencies (below 20 orders)**, followed by a steep decline. A smaller secondary peak is observed around **100 orders**, indicating the presence of a distinct group of highly loyal and frequent customers.
- The **Reorder Interval Distribution** exhibits two prominent peaks—around **7 days** and **30 days**—suggesting that customers commonly follow either a **weekly** or **monthly** grocery shopping cycle.
- The **Customer Ordering Behavior** scatter plot indicates that customers with shorter intervals between purchases generally place more orders, whereas customers with longer reorder intervals tend to have lower purchasing frequency.

### 🛒 Market Basket Analysis

- The Apriori algorithm generated **336 association rules**, revealing frequently purchased product combinations within customer transactions.
- The **Top 10 Products Bought Together** table highlights strong associations among fresh produce items, with combinations such as **Organic Cilantro & Limes**, **Organic Garlic & Organic Yellow Onion**, and **Raspberries & Strawberries** exhibiting some of the highest lift values.
- The average **Lift value of 1.57** indicates that many product pairs are purchased together more frequently than expected by chance, suggesting meaningful product relationships.
- The average **Confidence value of 0.13** suggests moderate predictive strength, meaning the occurrence of one product moderately increases the likelihood of purchasing its associated product.
- The **Support vs Confidence** scatter plot shows that most association rules have **low support (below 2%)** but varying confidence levels, indicating that while these product combinations are relatively less frequent, they still represent valuable cross-selling opportunities.
- These associations can be leveraged to improve **product recommendations, bundle promotions, shelf placement, and targeted marketing campaigns**, ultimately enhancing customer experience and increasing sales.

---

## 💡 Business Recommendations

Based on the analysis, the following recommendations can help improve customer engagement, operational efficiency, and sales performance:

### 🛍️ 1. Implement Product Bundle Recommendations

Leverage the association rules identified through Market Basket Analysis to recommend complementary products during checkout and create bundle offers. This can improve cross-selling opportunities and increase the average order value.

### ⏰ 2. Optimize Inventory During Peak Shopping Hours

Since customer orders peak between **9 AM and 3 PM**, inventory replenishment and warehouse staffing should be prioritized during these hours to ensure product availability and faster order fulfillment.

### 📅 3. Target Weekly and Monthly Shoppers

The reorder interval analysis reveals two major purchasing cycles—approximately **7 days** and **30 days**. Personalized reminders, discounts, or subscription offers can be scheduled around these intervals to encourage repeat purchases.

### 👥 4. Develop Customer Loyalty Strategies

A small group of customers places significantly more orders than the average customer. Rewarding these high-frequency shoppers through loyalty programs or exclusive offers can improve long-term customer retention.

### 🥬 5. Prioritize High-Demand Product Categories

Fresh produce products dominate customer purchases. Maintaining optimal inventory levels and ensuring consistent availability of these products can reduce stockouts and improve customer satisfaction.

### 📊 6. Strengthen Personalized Product Recommendations

Association rules with an average **Lift of 1.57** provide meaningful product relationships that can be integrated into recommendation systems, helping customers discover complementary products and increasing basket size.

---

## 📁 Repository Structure

```text
Quick-Commerce-Analytics/
│
├── Dashboard/
│   └── Quick_Commerce_Analytics.pbix
│
├── Dataset/
│   ├── aisles.csv
│   ├── departments.csv
│   ├── order_products__prior.csv
│   ├── orders.csv
│   └── products.csv
│
├── Python/
│   ├── cleaning.py
│   ├── merging.py
│   ├── marketbasket.py
│   ├── market_basket.py
│   └── clean_rules.py
│
├── Output/
│   ├── market_basket_rules_clean.csv
│   └── market_basket_rules.csv
│
└── README.md
```



