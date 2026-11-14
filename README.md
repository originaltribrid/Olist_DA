# Olist_DA
EDA of Olist(Brazilian E-Commerce Dataset)

# 🛒 Brazilian E-Commerce Public Dataset (Olist) - Exploratory Data Analysis

This is my first data analysis project exploring 100,000+ orders from Olist (a major Brazilian e-commerce department store) to see key business drivers, customer satisfaction trends, and geographic revenue distributions using Python.

---

## 🚀 Project Overview
In this project, I performed end-to-end Exploratory Data Analysis (EDA) on a complex relational e-commerce dataset containing customers, orders, order items, payments, and reviews. The goal was to transform raw multi-table data into actionable business insights that drive logistics efficiency and customer retention.

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Environment:** Jupyter Notebook (VS Code / Anaconda)
* **Libraries:** 
  * `pandas` & `numpy` (Data cleaning, manipulation, and merging)
  * `matplotlib` & `seaborn` (Data visualization and statistical plotting)

---
## 🗄️ Dataset Source
This project uses the official **Brazilian E-Commerce Public Dataset by Olist** hosted on Kaggle. 

* **Dataset Name:** Brazilian E-Commerce Public Dataset by Olist
* **Source Link:** [Kaggle - Olist Brazilian E-Commerce Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
* **Description:** The dataset contains information on 100,000 orders from 2016 to 2018 made at multiple marketplaces in Brazil, covering order status, pricing, payment, freight performance, customer locations, product attributes, and customer reviews.

> **Note:** Due to file size limits on GitHub, raw CSV files are not included in this repository. To run the notebook locally, please download the CSV files from the Kaggle link above and place them in your project directory.

---

## 📂 Project Architecture & Workflow
1. **Data Ingestion & Relational Merging:** Joined 5 core datasets (`orders`, `customers`, `order_items`, `payments`, and `reviews`) using unique primary/foreign keys (`order_id`, `customer_id`) to create a unified master DataFrame of **117k+ rows**.
2. **Data Cleaning & Preprocessing:** Handled missing values, formatted datetime columns, and filtered anomalies to ensure data integrity.
3. **Feature Engineering:** Created derived metrics such as `total_order_value` (Price + Freight) and `delivery_delay_days` (Estimated vs. Actual delivery timestamps).

---

## 📊 Key Insights & Findings

### 1. Logistics Impact on Customer Satisfaction
* **Delivery Speed is King:** Analysis revealed a strong correlation between early deliveries and high customer ratings. Orders delivered 13+ days ahead of estimated dates predominantly received **5-star ratings**, whereas delayed or close-cut deliveries triggered a sharp increase in **1-star reviews**.

### 2. Geographic Revenue Segmentation (GMV)
* **Regional Dominance:** Aggregated total revenue (Gross Merchandise Value) by state showed that **São Paulo (SP)** generates the highest commercial volume, serving as the primary hub for customer acquisition and logistics demand.

---

## 📈 Visualizations Included
* Bar charts analyzing the exact relationship between delivery delay days and customer review scores (1 to 5).
* Regional revenue distribution plots highlighting top-performing Brazilian states.

---

## ⚙️ How to Run the Project Locally
1. Clone this repository to your local machine:
   ```bash
   git clone [https://github.com/parth100904/olist-ecom-analysis.git](https://github.com/parth100904/olist-ecom-analysis.git)
Open your terminal or Jupyter Notebook in the project directory.

Ensure required libraries are installed:

Bash
pip install pandas numpy matplotlib seaborn
Run the Jupyter Notebook (.ipynb) cells sequentially to reproduce the data cleaning, merging, and visualizations.

👤 Author
Parth Srivastava

LinkedIn Profile: www.linkedin.com/in/parth-srivastava100
