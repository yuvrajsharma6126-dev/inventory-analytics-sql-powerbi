# Inventory Analytics: Solving Inventory Inefficiencies with Advanced SQL

## Urban Retail Co. — Data-Driven Inventory Optimization

An end-to-end data analytics project focused on identifying inventory inefficiencies, improving stock management, and generating actionable insights for better inventory planning and decision-making.

---

## 📌 Project Overview

Urban Retail Co. is a mid-sized, fast-growing retail chain operating across physical stores and e-commerce platforms, managing 5,000+ SKUs across multiple categories and regions.

The business faced several inventory-related challenges, including frequent stockouts, overstocking of slow-moving products, limited visibility into inventory performance, and reactive inventory decisions.

This project uses **MySQL and advanced SQL analytics** to transform raw operational data into structured insights that can support better inventory planning and business decisions.

---

## 🎯 Business Challenges

The project focuses on addressing the following inventory problems:

- Frequent stockouts of fast-moving products
- Overstocking of slow-moving items
- Limited visibility into inventory and supplier performance
- Reactive inventory decisions instead of proactive planning
- Difficulty identifying inventory inefficiencies across stores and SKUs

---

## 🚀 Project Objectives

The key objectives of the project are to:

- Identify inventory inefficiencies and blind spots
- Detect understocked and overstocked products
- Calculate data-driven reorder points
- Analyze inventory performance across SKUs, stores, and regions
- Classify fast- and slow-moving products
- Measure inventory turnover and aging
- Generate actionable inventory KPIs
- Support data-driven inventory planning and decision-making

---

# 🔄 Project Workflow

The project follows a structured **data-to-insight workflow**:

### 1. Data Collection

Raw datasets containing inventory, sales, orders, products, stores, weather, and forecast information are collected from CSV files.

### 2. Data Ingestion

The raw datasets are loaded into MySQL using the **Bronze Layer** and `LOAD DATA INFILE`.

This layer preserves the raw data and provides the foundation for further processing.

### 3. Data Cleaning & Preparation

The data is cleaned and standardized before analysis.

Key data-quality checks include:

- Removing duplicate records
- Deduplication using `ROW_NUMBER()`
- CTE-based data cleaning
- Trimming and standardizing string fields
- Validating product and store identifiers
- Removing duplicate weather records
- Checking date consistency across datasets

### 4. Data Modeling

The cleaned data is organized into a normalized relational structure containing:

- Products
- Stores
- Inventory
- Sales
- Orders
- Weather
- Forecasts

Primary and foreign keys are used to maintain relationships and referential integrity.

### 5. Advanced SQL Analysis

The cleaned and structured data is analyzed using advanced SQL techniques, including:

- Common Table Expressions (CTEs)
- Window functions
- Aggregations
- Conditional logic
- Historical sales analysis

### 6. Inventory Analysis

The analysis focuses on answering key inventory-management questions:

- Which products are currently low on stock?
- Which SKUs are overstocked?
- Which products are fast- or slow-moving?
- Which products require replenishment?
- How efficiently is inventory being utilized?
- What is the current inventory turnover?
- What are the key inventory performance indicators?

### 7. KPI Generation

Key inventory KPIs are calculated to evaluate inventory health and operational performance, including:

- Stockout rate
- Average inventory
- Inventory age
- Inventory turnover
- Stock availability

### 8. Business Insights & Visualization

The analytical results are converted into actionable business insights and presented through a **Power BI dashboard** for easier monitoring and decision-making.

---

# 📊 SQL Analysis

The project contains multiple analytical SQL scripts:

| SQL Script | Description |
|---|---|
| `stock_summary.sql` | Inventory rollups and under/overstock detection |
| `low_inventory.sql` | Identifies low-stock SKUs using 30-day sales history |
| `reorder_point.sql` | Calculates reorder points using 7-day demand |
| `turnover_ratio.sql` | Classifies inventory based on turnover |
| `kpi_summary.sql` | Calculates key inventory performance metrics |

---

# 💡 Key Business Insights

The analysis is designed to provide insights into:

- Low-stock and high-risk SKUs
- Overstocked and understocked inventory
- Fast- and slow-moving products
- Inventory aging
- Inventory turnover
- Reorder requirements
- Stock availability
- Overall inventory health

These insights can help businesses make more proactive inventory and replenishment decisions.

---

# 📈 Business Impact

The project aims to support:

- Data-driven reorder recommendations
- Earlier identification of low-stock products
- Better classification of fast- and slow-moving SKUs
- Improved inventory monitoring
- Reduced excess inventory and holding costs
- Better working-capital management
- Improved product availability
- More informed operational decision-making

---
<img width="1306" height="733" alt="image" src="https://github.com/user-attachments/assets/0e3fefd3-27cc-4652-b507-7554f01b6445" />
<img width="1318" height="735" alt="image" src="https://github.com/user-attachments/assets/06397f20-614b-447c-bb9e-b66eaeb1965c" />

# 📁 Project Structure

```text
inventory-analytics-sql-powerbi/
│
├── dataset/
│
├── scripts/
│   │
│   ├── bronze_ddl.sql
│   ├── proc_load_bronze.sql
│   │
│   ├── silver_ddl.sql
│   ├── proc_load_silver.sql
│   │
│   └── analysis/
│       ├── stock_summary.sql
│       ├── low_inventory.sql
│       ├── reorder_point.sql
│       ├── turnover_ratio.sql
│       └── kpi_summary.sql
│
├── solving_inventory_dashboard.pbit
├── EER_Diagram.pdf
├── MySQL Local.session.sql
└── README.md
