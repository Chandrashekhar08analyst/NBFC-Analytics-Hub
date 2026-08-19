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

The key business areas covered include **Business Performance, Collections & Recovery Behavior, Marketing Performance, risk Segment and Portfolio Performance**. The project also includes advanced analytics such as **Static Pool Cohort Analysis, Customer Lifetime Value & Cohort Analysis and Customer Segmentation** to identify recovery trends, customer retention patterns and high-value customer segments.

> **Data Note:** The project represents realistic NBFC business workflows. Company and product names used for public demonstration are fictional.

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="100%">
</p>

## Business Problem
The project addresses a common challenge in multi-product NBFC environments, where similar business data is maintained across different loan products, making it difficult to **keep data consistent, reduce manual effort, and compare product performance**.

### Solution
The project creates a **standardized analytical workflow** that integrates product-wise operational data into common business structures and applies reusable business logic, SQL analysis and reporting across products.

## Key Business Questions
The analytical system is designed to answer questions such as:
- Which loan products are driving business growth?
- How are disbursements and fresh vs repeat business performing?
- Which products and segments have stronger collection and recovery performance?
- Which products or segments carry higher NPA risk?
- Which marketing activities generate stronger lead and loan conversion?
- How does recovery performance vary across disbursement cohorts?
- Which customer segment and cohorts deliver higher long-term value?


<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="100%">
</p>

## 🏗️ Solution Architecture

<p align="center">
  <img width="1693" height="929" alt="NBFC Analytics Hub Architecture Pipeline" src="https://github.com/user-attachments/assets/3d9a879a-cbaf-4c44-beec-9b2154ce8e37" />

</p>

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="100%">
</p>

## Technology Used

| Category | Technology |
|---|---|
| **Programming** | Python|
| **Database** | PostgreSQL|
| **Data Engineering & Analytics** | Pandas, NumPy, Matplotlib |
| **Database Connectivity** | SQLAlchemy, psycopg2, python-dotenv |
| **Business Intelligence** | Power BI |
| **Data Source** | Microsoft Excel |
| **Development & Version Control** | Jupyter Notebook, GitHub |

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="100%">
</p>

# Project Execution Workflow

## 1. Data Integration
The project begins with **multiple product-wise Excel datasets** containing Leads, Disbursement, Collection, Master and Marketing information.

Since different products can maintain similar business information using different column names, formats or structures, the first step is to map the source data into a **common business schema**.

### Business Purpose
Instead of maintaining separate analysis workflows for every product, the integrated dataset allows the **same analytical logic to be applied across all products in one workflow**.


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


## 3. Data Synchronization
Relationships between Master, Disbursement, Collection and other datasets are validated to maintain consistency across the analytical system and prevent mismatched business values.


## 4. Feature Engineering
Raw operational data does not always contain all the fields required for business analysis. Therefore, additional analytical features are created during the ETL process. Examples include:
- Principal Recovered, Interest Recovered
- Repayment Bucket
- Age, Salary, Tenure, CIBIL Buckets and many more.
These features convert operational data into analysis-ready business information.


## 5. PostgreSQL Database Integration
The processed datasets are loaded into PostgreSQL using Python with:
- SQLAlchemy
- psycopg2
- python-dotenv

The processed DataFrames are automatically loaded into PostgreSQL tables using Python. Database credentials are stored in a local `.env` file instead of being hardcoded in the project.

### Business Purpose
PostgreSQL acts as the **centralized analytical database** for SQL analysis and Power BI reporting.


## 6. SQL Analysis & Reporting Layer

Processed PostgreSQL data is transformed into **reusable SQL queries and reporting views** for recurring business and management analysis.

SQL views also serve as **Power BI-ready datasets**, enabling consistent and refreshable reporting.

## 7. Power BI Integration & Dynamic Reporting

SQL reporting views are connected to **Power BI** to build interactive dashboards for monitoring **KPIs, trends and business performance**.

A simple **data refresh** updates the dashboards with the latest PostgreSQL data — **no dashboard rebuilding required**.

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="100%">
</p>

## Data Analysis

The analysis focuses on uncovering insights such as:
- **Business Growth & Performance**: Analyzing disbursement trends, cumulative growth, MoM performance, fresh vs repeat business and product contribution.
- **Collection & Recovery**: Measuring collection performance, recovery efficiency and repayment behaviour across products and customer segments.
- **Risk & NPA Segmentation**: Identifying NPA trends, delinquency buckets and high-risk products or customer segments.
- **Marketing Performance**: Evaluating leads, conversion, marketing spend, CAC and revenue contribution.
- **Executive Performance**: Providing a consolidated view of business, revenue, collection, marketing and portfolio risk.

Beyond standard reporting and dashboards, the project includes Python-based advanced analytics to understand deeper customer and portfolio behavior.
- Static Pool Cohort Analysis:
Analyzes recovery performance of disbursement cohorts over time to identify stronger and weaker recovery patterns.
- Customer Lifetime Value & Cohort Analysis:
Analyzes customer behavior across subsequent periods to understand repeat borrowing, customer retention and long-term customer value.
- Customer Segmentation:
Groups customers based on business value and behavior to identify high-value, repeat and strategically important customer segments.

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

## Dashboard Preview

<p align="center">
  <img width="1403" height="795" alt="Business Performance Dashboard" src="https://github.com/user-attachments/assets/82139a38-24b2-45a3-823c-ff10d4340557" />
</p>

<p align="center">
  <img width="1409" height="792" alt="Collection & Recovery Dashboard" src="https://github.com/user-attachments/assets/e2523a41-c8f7-47a1-8e32-00bf0740721e" />
</p>

<p align="center">
  <img width="1403" height="788" alt="Marketing Performance Dashboard" src="https://github.com/user-attachments/assets/5877b7a0-4cd1-418a-a9b9-128e8ffa6ddf" />
</p>

## 🎥 Interactive Dashboard Demo

**Dynamic Power BI Report Demo**

[▶️ Watch the Interactive Dashboard Demo](YOUR_VIDEO_LINK_HERE)

<p align="left">
  <img src="https://www.animatedimages.org/data/media/562/animated-line-image-0184.gif" width="100%">

</p>

## Conclusion

**NBFC Analytics Hub** demonstrates how raw multi-product operational data can be transformed into a centralized, reusable analytics workflow covering **data integration, data quality, database management, SQL reporting, business intelligence and advanced portfolio analytics**.

**From Raw Data → Standardized Pipeline → PostgreSQL → SQL Analytics → Power BI → Business Intelligence**

---

<p align="center">
  <b>NBFC Analytics Hub — Loan Portfolio Intelligence</b>
  <br>
  <i>From Raw Data to Business Intelligence</i>
</p>

<p align="center">
  <i>Built with Python · PostgreSQL · SQL · Power BI · Excel · Analytical Libraries like Pandas, NumPy, Matplotlib & SqlAlchemy</i>
</p>
