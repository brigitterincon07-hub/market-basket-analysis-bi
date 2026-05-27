# Market Basket Analysis for Retail Assortment Optimization

## 📌 Business Overview
This project develops a **Recommendation Engine** for grocery retail using transactional data (9,835 transactions and 169 unique products). By applying the **Apriori Algorithm** and **Association Rules**, the goal is to discover hidden patterns in consumer purchasing behavior to optimize product placement, cross-selling strategies, and inventory assortment.

## 📊 Key Insights & Exploratory Data Analysis (EDA)
* **Purchase Volume:** The average transaction contains **4 items**, and 90% of customers purchase a maximum of 9 products per visit.
* **Top Sellers:** `Whole milk` (25.55%) and `other vegetables` (19.34%) are the high-frequency anchor items in the store.

## 🛠️ Methodology & Tech Stack
* **Language:** Python 3
* **Libraries:** `pandas`, `matplotlib`, `seaborn`, `mlxtend` (Frequent Patterns)
* **Algorithm:** Apriori Framework
* **Data Transformation:** One-Hot Encoding via `TransactionEncoder` to build a sparse logical matrix.
* **Rule Optimization:** Filtered rules by setting a minimum support threshold based on item occurrences ($N \ge 30$) and evaluated using **Confidence** and **Lift** metrics.

## 📈 Practical Business Applications (Results)
* **Targeted Cross-Selling:** Strong predictive rules were identified. For instance, when a customer adds `rice` to their cart, there is a **61.33% confidence** that they will also buy `whole milk` (Lift: 2.40) and a **52% confidence** they will buy `other vegetables` (Lift: 2.68).
* **Strategic Shelf Placement:** Anchor categories like `other vegetables` are strongly driven by combined antecedent purchases of `root vegetables`, `citrus fruit`, and `tropical fruit` (Confidence: 78.5%, Lift: 4.06). 

## 🚀 How to Open in Google Colab
You can run this notebook directly in Google Colab by clicking the link inside the repository.
