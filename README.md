# NBFC Analytics Hub 🏦 | Loan Portfolio Intelligence Analytics

<p align="center">
  <img src="https://img.shields.io/badge/Status-Completed-1F6FEB?style=for-the-badge" alt="Status">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/SQL-336791?style=for-the-badge&logo=postgresql&logoColor=white" alt="Analytical Libraries">
  <img src="https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI">
  <img src="https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white" alt="Excel">
</p>

<p align="center">
  <b>Python</b> · <b>PostgreSQL</b> · <b>Analytical Libraries</b> · <b>Power BI</b> · <b>Excel</b>
  <br>
  Pandas · NumPy · Matplotlib · SQLAlchemy · psycopg2 · python-dotenv
</p>

<p align="center">
  <i>End-to-End NBFC Data Engineering Pipeline & Analytical Workflow Platform</i>
</p>

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="100%">
</p>

## Introduction

The **NBFC Analytics Hub** is an end-to-end **Data Engineering and Analytics Platform** designed to cover the complete NBFC data analytics lifecycle — from raw multi-product data to integrated data pipelines, centralized database storage, business analysis, dynamic Power BI dashboards and advanced analytics.

The project addresses a common challenge in multi-product NBFC environments, where similar business data is maintained across different loan products and often requires separate data preparation and reporting processes. This project brings the data into a **standardized analytical workflow**, enabling consistent analysis across products.

The key business areas covered include **Business Performance, Collections & Recovery Behavior, Marketing Performance, risk Segment and Portfolio Performance**.

The project also includes advanced analytics such as **Static Pool Cohort Analysis, Customer Lifetime Value & Cohort Analysis and Customer Segmentation** to identify recovery trends, customer retention patterns and high-value customer segments.

> **Data Note:** The project represents realistic NBFC business workflows. Company and product names used for public demonstration are fictional.

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="100%">
</p>

## Architecture

<p align="center">
  <img src="./assets/architecture.png" alt="NBFC Analytics Hub Architecture" width="900">
</p>

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="100%">
</p>

## Technology Used

| Category | Technology |
|---|---|
| Programming | Python |
| Data Processing | Pandas, NumPy |
| Visualization / Analytics | Matplotlib |
| Database | PostgreSQL |
| Database Connectivity | SQLAlchemy, psycopg2 |
| Query Language | SQL |
| Business Intelligence | Power BI |
| Raw Data Source | Microsoft Excel |
| Development Environment | Jupyter Notebook |
| Credential Management | python-dotenv |
| Version Control | Git & GitHub |

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="100%">
</p>

# Project Execution Workflow

## 1. Data Integration
The project begins with **multiple product-wise Excel datasets** containing Leads, Disbursement, Collection, Master and Marketing information.

Since different products can maintain similar business information using different column names, formats or structures, the first step is to map the source data into a **common business schema**.

### Business Purpose
Instead of maintaining separate analysis workflows for every product, the integrated dataset allows the **same analytical logic to be applied across all products in one workflow**.

---

## 2. Data Cleaning & Standardization
The integrated datasets are cleaned and validated before any business analysis is performed.

Key activities include:
- Handling missing values
- Removing duplicate records
- Correcting data types
- Removing unwanted spaces
- Standardizing categorical values
- Correcting spelling inconsistencies
- Validating business rules

---

## 3. Data Synchronization
This ensures that information across Master, Collection and other related datasets remains consistent and prevents mismatched business values during analysis.

---

## 4. Feature Engineering
Raw operational data does not always contain all the fields required for business analysis. Therefore, additional analytical features are created during the ETL process.

Examples include:
- Principal Recovered, Interest Recovered
- Repayment Bucket
- Age, Salary, Tenure, CIBIL Buckets and many more.
These features convert operational data into analysis-ready business information.

---

## 5. PostgreSQL Database Integration
The processed datasets are loaded into PostgreSQL using Python with:
- SQLAlchemy
- psycopg2
- python-dotenv

The processed DataFrames are automatically loaded into PostgreSQL tables using Python.

Database credentials are stored in a local `.env` file instead of being hardcoded in the project.

### Business Purpose
PostgreSQL acts as the **centralized analytical database** for SQL and Power BI to get specific data.

---

## 6. SQL Analysis & Reporting Layer
Once the processed data is available in PostgreSQL, SQL is used to create **reusable analysis queries and reporting views**.

### Business Purpose
The queries work with the latest PostgreSQL data, allowing **updated analytical and monthly management reports** to be generated without rebuilding the analysis.

SQL views also serve as **Power BI-ready datasets**. After updating the views and performing a **Power BI data refresh**, the dashboards reflect the latest available data.

This creates a **consistent, reusable and efficient reporting workflow**.


---

## 7. Power BI Integration & Dynamic Dashboard

The SQL reporting views are connected to **Power BI** to build interactive dashboards and reports that provide stakeholders with **actionable business insights**.

The visualizations help identify key **patterns, trends and performance changes**, making data-driven decision-making easier.

Once the underlying data and SQL views are updated, a simple **Power BI data refresh** updates the dashboards with the latest available information — **no dashboard rebuilding is required**.


---

## 8. Advanced NBFC Analytics

Beyond standard reporting and dashboards, the project includes Python-based advanced analytics to understand deeper customer and portfolio behaviour.

### Static Pool Cohort Analysis

Analyzes recovery performance of disbursement cohorts over time to identify stronger and weaker recovery patterns.

### Customer Lifetime Value & Cohort Analysis

Analyzes customer behavior across subsequent periods to understand repeat borrowing, customer retention and long-term customer value.

### Customer Segmentation

Groups customers based on business value and behavior to identify high-value, repeat and strategically important customer segments.

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="100%">
</p>

## Data Analysis

The analysis focuses on uncovering insights such as:
- **Business Growth & Performance**: Analyzing disbursement trends, cumulative growth, MoM performance, fresh vs repeat business and product contribution.
- **Collection & Recovery**: Measuring collection performance, recovery efficiency and repayment behaviour across products and customer segments.
- **Risk & NPA Segmentation **: Identifying NPA trends, delinquency buckets and high-risk products or customer segments.
- **Marketing Performance**: Evaluating leads, conversion, marketing spend, CAC and revenue contribution.
- **Executive Performance**: Providing a consolidated view of business, revenue, collection, marketing and portfolio risk.
- **Static Pool Cohorts**: Comparing recovery performance across different disbursement cohorts over time.
- **Customer Lifetime Value**: Identifying customers and segments with stronger long-term business value.
- **Customer Segmentation**: Understanding customer groups based on value, behaviour and repeat-borrowing patterns.

The analysis helps answer key business questions such as **which products are performing better, where recovery is stronger, which segments carry higher risk, which marketing activities generate better outcomes and which customers provide stronger long-term value**.

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="100%">
</p>

## Data Visualization & Power BI Dashboards

The analytical results are visualized using **Microsoft Power BI**, providing interactive dashboards for monitoring business performance, collections, marketing, risk and executive-level KPIs.

The dashboards include:

- **Business Performance Dashboard**
- **Collection & Recovery Dashboard**
- **Marketing Performance Dashboard**
- **NPA & Risk Dashboard**
- **Executive Performance Dashboard**

The dashboards use **dynamic KPIs, filters, charts and interactive visuals** to help stakeholders explore trends, compare segments and make data-driven decisions.

### Dashboard Preview

<p align="center">
  <img src="./assets/business_performance.png" alt="Business Performance Dashboard" width="48%">
  <img src="./assets/collection_recovery.png" alt="Collection & Recovery Dashboard" width="48%">
</p>

<p align="center">
  <img src="./assets/marketing_performance.png" alt="Marketing Performance Dashboard" width="48%">
  <img src="./assets/risk_analysis.png" alt="NPA & Risk Dashboard" width="48%">
</p>

<p align="center">
  <img src="./assets/executive_performance.png" alt="Executive Performance Dashboard" width="70%">
</p>

> Replace the image paths above with your actual Power BI dashboard screenshots.

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="100%">
</p>

## Conclusion

The **NBFC Analytics Hub** demonstrates a complete end-to-end **Data Engineering and Analytics workflow** for a multi-product NBFC environment. The project transforms raw product-wise data into a centralized analytical system through **data integration, cleaning, standardization, synchronization, feature engineering, PostgreSQL and SQL-based reporting**, followed by dynamic Power BI dashboards and advanced analytics.

The combination of **reusable SQL analysis, automated reporting, interactive dashboards and advanced customer and portfolio analytics** provides a comprehensive view of business growth, collection performance, marketing efficiency, portfolio risk and customer behaviour.

Overall, the project demonstrates how a structured data pipeline can transform raw operational NBFC data into **reusable business intelligence for faster and more informed decision-making** by **Automating Repeating Work**.

---

<p align="center">
  <b>NBFC Analytics Hub — Loan Portfolio Intelligence</b>
  <br>
  <i>From Raw Data to Business Intelligence</i>
</p>

<p align="center">
  <i>Built with Python · PostgreSQL · SQL · Power BI · Excel · Analytical Libraries like Pandas, NumPy, Matplotlib & SqlAlchemy</i>
</p>
