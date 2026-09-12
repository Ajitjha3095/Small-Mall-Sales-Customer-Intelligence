<div align="center">

<img width="648" height="464" alt="image" src="https://github.com/user-attachments/assets/47772cce-8a5a-4f50-9ab7-427f0434b89d" />

<img width="757" height="423" alt="image" src="https://github.com/user-attachments/assets/3bbcbf30-4c17-4e10-b0c0-b7efd768a57a" />



# 🏬 Small Mall — Sales & Customer Intelligence

### End-to-End Data Analytics, Business Intelligence & Graph Analytics Portfolio Project

> **Project period:** 2024–2026  
> **Business context:** One shopping mall with multiple shops
> **Dataset size:** 2,000 synthetic transaction records

---
###   

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-KPI%20Measures-5E5E5E?style=for-the-badge)
![Data Modeling](https://img.shields.io/badge/Data%20Modeling-Relationships-2F855A?style=for-the-badge)
![Looker Studio](https://img.shields.io/badge/Looker%20Studio-4285F4?style=for-the-badge)
![Neo4j](https://img.shields.io/badge/Neo4j-Graph%20DB-008CC1?style=for-the-badge)
![Cypher](https://img.shields.io/badge/Cypher-Query%20Language-2F855A?style=for-the-badge)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

> A complete end-to-end analyst portfolio project built across three industry-standard BI platforms and a graph database layer.
> Python (Data Extraction) → Raw Data → Cleaning → Modeling → Power BI · Tableau · Looker Studio → Neo4j → Cypher

</div>

## Live Demos

A single-page BI dashboard analyzing public WiFi subscriber behavior, churn risk, and revenue leakage for Q2 2026 — built in Power BI, Tableau, and Looker Studio from the same dataset.



| Platform | Link |
|---|---|
| Power BI | See `/Dashboard` folder (`.pbix` file) |
| Tableau Public | [MallSalesCustomerIntelligence2024-2026](https://public.tableau.com/app/profile/ajit.jha/viz/MallSalesCustomerIntelligence2024-2026/Dashboard1?publish=yes) |
| Looker Studio | [Live Report](https://datastudio.google.com/s/m_RwL8QXXcQ) |
| GitHub Repo | [Ajitjha3095/Small-Mall-Sales-Customer-Intelligence](https://github.com/Ajitjha3095/Small-Mall-Sales-Customer-Intelligence) |
| Neo4j Cypher | See `/Cypher query` folder  |


---

## 📌 Executive Summary

**Small Mall — Sales & Customer Intelligence** is an end-to-end analytics portfolio project demonstrating how raw transactional data can be transformed into business insights and relationship-based intelligence.

The project uses **Python and Pandas** for data preparation and validation, **Power BI, Tableau, and Looker Studio** for business intelligence and visualization, and **Neo4j** for graph modeling and relationship analysis.

The solution covers:

- Data preparation and quality validation
- Retail sales and customer analysis
- KPI development and dashboard design
- Shop, product, and category performance
- Graph data modeling and Cypher analysis

---

## 🎯 Business Problem

Mall management needs a consolidated view of sales performance and customer activity across multiple shops.

This project addresses questions such as:

- How is revenue changing from 2024 to 2026?
- Which shops generate the highest revenue?
- Which shops have the strongest profitability?
- Which categories and products contribute most to sales?
- What is the average transaction value?
- How many unique customers are purchasing?
- Which payment methods generate the most revenue?
- Which customers purchase from multiple shops?
- Which shops share the same customer base?

---

## 💼 Project Objectives

1. Create a synthetic retail dataset.
2. Inspect and validate the raw data using Pandas.
3. Clean and transform the dataset.
4. Export a cleaned master CSV.
5. Split the data into analytical files.
6. Build a recruiter-focused Power BI dashboard.
7. Create Tableau and Looker Studio reports.
8. Model business relationships in Neo4j.
9. Use Cypher queries for graph analysis.
10. Publish the project through GitHub and Kaggle.

---

## 🏗️ Solution Architecture

```text
                    Synthetic Raw CSV
                           │
                           ▼
                    Python / Pandas
                           │
             Data Inspection & Validation
                           │
                           ▼
                 Cleaned Master Dataset
                           │
             ┌─────────────┴─────────────┐
             │                           │
             ▼                           ▼
     Business Intelligence         Graph Analytics
             │                           │
     ┌───────┼────────┐                  ▼
     ▼       ▼        ▼                Neo4j
  Power BI Tableau Looker              Cypher
```

---

## 📂 Repository Structure

```text
Small-Mall-Sales-Customer-Intelligence/
│
├── DataSet/
│   ├── mall_raw_data_2024_2026.csv
│   ├── mall_cleaned_data_2024_2026.csv
│   ├── customers.csv
│   ├── shops.csv
│   └── transactions.csv
│
├── Jupyter_Notebook/
│   └── 01_Data_Cleaning.ipynb
│
├── PowerBI/
│   └── Small_Mall_Sales_Customer_Intelligence.pbix
│
├── Tableau/
│   └── Small Mall — Sales & Customer Intelligence.twb
│
├── Looker/
│   └── Dashboard_Reference.md
│
├── Neo4j/
│   └── Cypher/
│
└── README.md
```

---

## 📊 Dataset Overview

| Attribute | Details |
|---|---|
| Business Context | Single shopping mall |
| Time Period | 2024–2026 |
| Records | 2,000 |
| Raw Columns | 13 |
| Dataset Type | Synthetic |
| File Format | CSV |
| Shops | Multiple |
| Customers | Multiple |
| Categories | Multiple |
| Transaction ID | Not used |

---

## 📋 Data Dictionary

| Column | Description |
|---|---|
| `Date` | Date of the transaction |
| `Customer_ID` | Customer identifier |
| `Shop_ID` | Shop identifier |
| `Shop_Name` | Name of the shop |
| `Category` | Product or shop category |
| `Product_Name` | Purchased product |
| `Quantity` | Number of units purchased |
| `Unit_Price` | Price per unit |
| `Discount` | Applied discount value |
| `Sales_Amount` | Final sales amount |
| `Payment_Method` | Payment method used |
| `Customer_Type` | Customer membership/type classification |
| `Rating` | Customer rating |

---

## 🐼 Data Preparation — Python & Pandas

### Workflow

```text
Raw CSV
   │
   ▼
Load Dataset
   │
   ▼
Inspect Shape and Data Types
   │
   ▼
Check Missing Values
   │
   ▼
Check Duplicate Records
   │
   ▼
Convert Date and Numeric Fields
   │
   ▼
Validate Numerical Values
   │
   ▼
Validate Sales Amount
   │
   ▼
Create Cleaned Master Dataset
   │
   ▼
Split Analytical Files
```

### Preparation Activities

- CSV ingestion using Pandas
- Dataset structure inspection
- Missing-value validation
- Duplicate checking
- Data-type validation
- Date conversion
- Numeric field validation
- Sales amount validation
- Data transformation
- Master dataset export
- Analytical dataset splitting

---

## 📁 Data Model

The cleaned master dataset was separated into three focused files for structured analysis and Neo4j modeling.

```text
mall_cleaned_data_2024_2026.csv
              │
       ┌──────┼─────────┐
       ▼      ▼         ▼
 customers  shops  transactions
```

### `customers.csv`

```text
Customer_ID
Customer_Type
```

### `shops.csv`

```text
Shop_ID
Shop_Name
Category
```

### `transactions.csv`

```text
Date
Customer_ID
Shop_ID
Product_Name
Quantity
Unit_Price
Discount
Sales_Amount
Payment_Method
Rating
```

---

# 📊 Power BI — Sales & Customer Intelligence

The Power BI dashboard provides an executive-level view of mall performance.

### Key KPIs

- Total Revenue
- Average Transaction Value
- Unique Customers
- Average Rating
- Profit Margin %

### Key Visuals

- Revenue and Profit Trend
- Revenue by Category
- Revenue by Payment Method
- Highest-Selling Products
- Shop Performance Matrix
- Category, Shop, and Product slicers

### Analytical Focus

- Revenue performance
- Profitability
- Shop contribution
- Product performance
- Customer activity
- Payment behavior
- Category performance

---

# 📈 Tableau — Interactive Visual Analytics

Tableau provides an additional interactive visualization layer using the same business dataset.

### Analysis Areas

- Revenue trends
- Shop performance
- Product performance
- Category contribution
- Customer analysis
- Sales distribution
- Interactive filtering

---

# 📉 Looker Studio — Web-Based Reporting

Looker Studio provides a browser-based reporting experience.

### Analysis Areas

- Revenue overview
- Customer metrics
- Shop performance
- Product performance
- Category analysis
- Interactive filters
- Business performance monitoring

---

# 🕸️ Neo4j — Graph Analytics

The project uses Neo4j to model relationships between customers, transactions, shops, products, and categories.

## Graph Entities

### Nodes

- `Customer`
- `Transaction`
- `Shop`
- `Product`
- `Category`

### Relationships

- `MADE`
- `PURCHASED_FROM`
- `CONTAINS`
- `BELONGS_TO`

## Graph Model

```text
(Customer)
     │
     │ MADE
     ▼
(Transaction)
     │
     ├── PURCHASED_FROM ──► (Shop)
     │
     └── CONTAINS ────────► (Product)

(Shop)
     │
     │ BELONGS_TO
     ▼
(Category)
```

## Graph Questions

- Which customers purchase from multiple shops?
- Which shops share customers?
- Which products are associated with specific shops?
- Which categories attract the most customers?
- Which entities are highly connected?
- What are the strongest customer-to-shop relationships?

---

## 🧮 Key Business Metrics

### Total Revenue

```text
Total Revenue = SUM(Sales_Amount)
```

### Average Transaction Value

```text
Average Transaction Value =
Total Revenue / Total Transactions
```

### Revenue per Customer

```text
Revenue per Customer =
Total Revenue / Unique Customers
```

### Profit Margin

```text
Profit Margin =
Total Profit / Total Revenue
```

Additional metrics include:

- Revenue Growth %
- Revenue Contribution %
- Shop Revenue Rank
- Product Revenue Rank
- Customer Segmentation
- Transaction Volume
- Average Rating
- Payment Method Contribution

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Data creation and preparation |
| Pandas | Data cleaning and transformation |
| Jupyter Notebook | Data preparation |
| Power BI | Business intelligence dashboard |
| DAX | KPI and analytical calculations |
| Tableau | Interactive visualization |
| Looker Studio | Web-based reporting |
| Neo4j | Graph database and analytics |
| Cypher | Graph querying |
| CSV | Data storage |
| GitHub | Version control and documentation |
| Kaggle | Dataset publishing |

---

## 📌 Skills Demonstrated

### Data Analytics

- Data inspection
- Data cleaning
- Data validation
- Data transformation
- Exploratory analysis
- KPI development
- Business problem solving

### Business Intelligence

- Power BI dashboard development
- DAX measures
- KPI design
- Interactive slicers
- Matrix visuals
- Conditional formatting
- Business storytelling

### Graph Analytics

- Property graph modeling
- Nodes and properties
- Relationships
- Cypher queries
- Pattern matching
- Relationship-based business analysis

---

## 🔄 End-to-End Workflow

```text
1. Create Synthetic Dataset
        ↓
2. Save Raw CSV
        ↓
3. Load Data with Pandas
        ↓
4. Inspect Data Structure
        ↓
5. Validate Data Quality
        ↓
6. Clean and Transform Data
        ↓
7. Export Cleaned Master CSV
        ↓
8. Split Analytical Files
        ↓
9. Build Power BI Dashboard
        ↓
10. Build Tableau Dashboard
        ↓
11. Build Looker Studio Report
        ↓
12. Create Neo4j Graph Model
        ↓
13. Execute Cypher Queries
        ↓
14. Publish Project and Dataset
```

---

## 🔗 Project Resources

Replace the placeholders with your actual links.

| Resource | Link |
|---|---|
| Kaggle Dataset | `Add Kaggle URL` |
| Power BI Dashboard | `Add Power BI URL or file reference` |
| Tableau Public | `Add Tableau URL` |
| Looker Studio | `Add Looker Studio URL` |
| Neo4j Project | `Add Neo4j/GitHub URL` |

---

## 📷 Dashboard Preview

Add screenshots to an `assets` folder and update the filenames below.

```markdown
![Power BI Dashboard](assets/powerbi-dashboard.png)

![Tableau Dashboard](assets/tableau-dashboard.png)

![Looker Studio Dashboard](assets/looker-dashboard.png)

![Neo4j Graph Model](assets/neo4j-graph.png)
```

---

## 📈 Business Value

Although the dataset is synthetic, the project follows a practical business intelligence workflow.

It demonstrates how organizations can use:

- Structured sales data for performance reporting
- Customer-level data for customer intelligence
- Shop-level data for retail benchmarking
- Product-level data for demand analysis
- Graph data for relationship discovery

The project demonstrates the ability to move from **raw data to business insight**, while supporting both structured analytics and graph analytics.

---

## ⚠️ Dataset Disclaimer

This dataset is synthetic and was created for educational, portfolio, and data analytics practice purposes.

It does not represent real customers, real businesses, real transactions, or confidential financial information.

---

## 👨‍💻 Author

### Ajit Jha

**Data Analyst | Business Intelligence | Data Visualization**

If you find the analytical approach useful, feel free to explore the repository and dashboards.

- **GitHub:** [Ajitjha3095](https://github.com/Ajitjha3095)
- **LinkedIn:** [Ajit Jha](https://www.linkedin.com/in/ajitjha01/)

**Core Skills**

`Python` · `Pandas` · `SQL` · `Power BI` · `DAX` · `Tableau` · `Looker Studio` · `Neo4j` · `Cypher`

---

## ⭐ Project Highlights

- End-to-end analytics workflow
- 2,000 synthetic retail records
- Single-mall, multi-shop business context
- Python and Pandas data preparation
- Power BI executive dashboard
- Tableau interactive analysis
- Looker Studio web reporting
- Neo4j graph modeling
- Structured and graph-based analytics
- GitHub and Kaggle portfolio publishing

---
