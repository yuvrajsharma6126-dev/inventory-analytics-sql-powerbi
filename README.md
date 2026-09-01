# Inventory Analytics: Solving Inventory Inefficiencies with Advanced SQL

## Urban Retail Co. — Data-Driven Inventory Optimization

An end-to-end SQL analytics project focused on identifying inventory inefficiencies, improving stock management, and generating actionable insights for better inventory planning.

---

## 📌 Project Overview

Urban Retail Co. is a mid-sized retail business operating across physical stores and e-commerce channels, managing 5,000+ SKUs across multiple categories and regions.

The business faces common inventory challenges such as stockouts, overstocking, limited visibility into inventory performance, and reactive replenishment decisions.

This project uses **MySQL, advanced SQL analytics, and a structured three-layer data pipeline** to transform raw inventory data into actionable business insights.

---

## 🎯 Business Challenges

The analysis focuses on addressing the following problems:

- Frequent stockouts of fast-moving products
- Overstocking of slow-moving inventory
- Limited visibility into SKU, store, and supplier performance
- Reactive rather than data-driven inventory planning
- Difficulty identifying inventory blind spots
- Lack of standardized inventory KPIs

---

## 🚀 Project Objectives

The project aims to:

- Identify understocked and overstocked products
- Calculate data-driven reorder points
- Analyze inventory performance across SKUs, stores, and regions
- Identify fast- and slow-moving products
- Evaluate inventory turnover and aging
- Generate operational KPIs for inventory management
- Build a scalable SQL analytics workflow

---

# 🏗️ Solution Architecture

The project follows a **three-layer SQL analytics architecture** implemented using MySQL:

```text
Raw CSV Data
     │
     ▼
┌──────────────────────┐
│   Bronze Layer       │
│ Raw Data Ingestion   │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│   Silver Layer       │
│ Data Cleaning &      │
│ Normalization        │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│  Analytical Layer    │
│ SQL Analysis & KPIs  │
└──────────┬───────────┘
           │
           ▼
   Business Insights
<img width="1375" height="750" alt="image" src="https://github.com/user-attachments/assets/9a4acaf7-91e2-4c12-8167-79c566743bf5" />
<img width="1343" height="742" alt="image" src="https://github.com/user-attachments/assets/ea607d47-b581-446d-aee8-fffae2cdb0c4" />
