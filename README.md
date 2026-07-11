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
><img width="374" height="212" alt="image" src="https://github.com/user-attachments/assets/e4922013-7fbb-4dd6-a23a-33d4fc0973a6" />



