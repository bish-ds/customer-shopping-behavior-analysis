# 🛒 Customer Shopping Behavior Analysis
### End-to-End Data Analytics Project | Python · SQL · Power BI

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Power BI](https://img.shields.io/badge/PowerBI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Wrangling-150458?style=for-the-badge&logo=pandas&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

---

## 📌 Project Overview

This project delivers a **corporate-grade, end-to-end data analytics workflow** on retail customer shopping behavior — covering every stage from raw data ingestion to executive-ready dashboards and reporting.

The goal is to uncover **actionable insights** around customer segments, purchase drivers, loyalty patterns, and revenue trends using a combination of Python, SQL, and Power BI.

---

## 🎯 Business Problem

Retail businesses often struggle to understand *why* customers buy, *who* their most valuable segments are, and *what* drives repeat purchases. This project simulates a real analyst's workflow to answer those questions with data.

**Key business questions answered:**
- Which customer segments generate the most revenue?
- Do subscribed customers spend more than non-subscribers?
- What products drive the highest discount uptake?
- How does shipping preference correlate with spend?
- Which age groups contribute the most to total revenue?

---

## 🏗️ Project Architecture

```
Raw CSV Data
    │
    ▼
┌──────────────────────────────┐
│  Python (Jupyter Notebook)   │
│  • Data Import & Exploration │
│  • Data Cleaning & EDA       │
│  • Load Data → SQL Database  │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│         SQL (PostgreSQL)     │
│  • Business Q&A Queries      │
│  • Customer Segmentation     │
│  • Revenue & Loyalty Analysis│
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│         Power BI             │
│  • Interactive Dashboard     │
│  • KPI Cards & Trend Charts  │
│  • Stakeholder-ready Report  │
└──────────────────────────────┘
```

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **Python** (Pandas, NumPy, Matplotlib, Seaborn, SQLAlchemy) | Data cleaning, EDA, database loading |
| **SQL** (PostgreSQL) | Business analysis queries, customer segmentation |
| **Power BI** | Interactive dashboard & data visualization |
| **Jupyter Notebook** | Reproducible analysis environment |

---

## 📂 Repository Structure

```
📦 customer-shopping-behavior-analysis
 ┣ 📓 Customer_Shopping_Behavior_Analysis.ipynb   # Python EDA & data loading
 ┣ 🗄️  customer_behavior_sql_queries.sql          # 10 business SQL queries
 ┣ 📊 customer_behavior_dashboard.pbix            # Power BI dashboard
 ┣ 📄 customer_shopping_behavior.csv              # Source dataset (3,900 records)
 ┣ 📋 Business Problem Document.pdf               # Project brief & business context
 ┣ 📑 Customer Shopping Behavior Analysis.pdf     # Full project report
 ┣ 🖥️  Customer-Shopping-Behavior-Analysis.pptx   # Stakeholder presentation deck
 ┗ 📜 README.md
```

---

## 📊 Key Insights

- 💰 **Subscription Impact**: Subscribed customers showed notably higher average spend, suggesting loyalty programs drive revenue.
- 👗 **Top Categories**: Clothing and Accessories dominated purchase volume across all segments.
- 🎁 **Discount Behavior**: A significant portion of high-spend customers *still used discounts*, indicating price-sensitive even among premium buyers.
- 👥 **Loyal Segment**: Customers with >10 previous purchases formed a small but highly valuable cohort.
- 🚚 **Shipping Preference**: Standard shipping correlated with slightly higher purchase amounts than Express.

---

## 🚀 How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/customer-shopping-behavior-analysis.git
cd customer-shopping-behavior-analysis
```

### 2. Set Up Python Environment
```bash
pip install pandas numpy matplotlib seaborn sqlalchemy psycopg2 jupyter
jupyter notebook
```

### 3. Run the Jupyter Notebook
Open `Customer_Shopping_Behavior_Analysis.ipynb` and run all cells to:
- Explore and clean the dataset
- Load data into your SQL database

### 4. Run SQL Queries
- Create a database (PostgreSQL recommended)
- Open `customer_behavior_sql_queries.sql`
- Execute queries to answer the 10 business questions

### 5. Open the Power BI Dashboard
- Open `customer_behavior_dashboard.pbix` in Power BI Desktop
- Connect to your local SQL database
- Explore the interactive dashboard

---

## 📁 Dataset

- **Source**: Customer Shopping Behavior Dataset
- **Records**: ~3,900 transactions
- **Features**: Age, Gender, Purchase Amount, Category, Item Purchased, Review Rating, Subscription Status, Shipping Type, Discount Applied, Previous Purchases, and more.

---

## 💡 SQL Analysis Highlights

10 business-driven SQL queries including:

| # | Query | Technique |
|---|-------|-----------|
| 1 | Revenue by Gender | GROUP BY, SUM |
| 2 | Discount users above avg spend | Subquery, WHERE |
| 3 | Top 5 highest-rated products | AVG, ORDER BY, LIMIT |
| 4 | Standard vs Express shipping spend | CASE, AVG |
| 5 | Subscriber vs non-subscriber revenue | GROUP BY, COUNT |
| 6 | Top discount-driven products | CASE WHEN, ROUND |
| 7 | Customer segmentation (New/Returning/Loyal) | CTE, CASE WHEN |
| 8 | Top 3 products per category | CTE, Window Functions, ROW_NUMBER |
| 9 | Repeat buyers & subscription correlation | WHERE, GROUP BY |
| 10 | Revenue by age group | GROUP BY, SUM |

---

## 📜 License

This project is licensed under the **MIT License** — feel free to fork, adapt, and use in your own portfolio.

---

## 🤝 Connect

If you found this project useful, feel free to ⭐ star it and connect!

> Built as a portfolio project demonstrating real-world data analytics skills across the full analytics stack.
