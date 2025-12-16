SQL Data Warehouse Project

A modern Data Warehouse solution built from scratch using SQL Server, following the Medallion Architecture (Bronze, Silver, Gold). This project demonstrates an end-to-end data engineering pipeline, transforming raw ERP and CRM data into actionable insights.

🚀 Project Overview

The goal of this project is to build a scalable and performant data warehouse that serves as a "Single Source of Truth" for business intelligence. It handles data ingestion, cleaning, transformation, and modeling to support reporting needs.

🏗️ Architecture (Medallion)

🥉 Bronze Layer (Raw): Direct ingestion of raw CSV data from source systems (ERP & CRM). Data is stored "as-is" to ensure a complete historical record.

🥈 Silver Layer (Cleaned): Data cleaning, standardization, and normalization. This layer handles null values, duplicates, and data type casting.

🥇 Gold Layer (Business): A refined Star Schema (Fact & Dimension tables) optimized for reporting and analytical queries.

🛠️ Technologies Used

Database: Microsoft SQL Server

Language: T-SQL (Transact-SQL)

ETL: Stored Procedures & SQL Scripts

Data Modeling: Star Schema (Facts & Dimensions)

Visualization: Power BI (optional integration)

📂 Project Structure

├── datasets/           # Raw CSV files (ERP & CRM data)
├── scripts/
│   ├── bronze/         # DDL & Stored Procedures for raw data ingestion
│   ├── silver/         # Transformation logic (cleaning, standardization)
│   ├── gold/           # View definitions for Fact & Dimension tables
│   └── init_database.sql
├── docs/               # Architecture diagrams and data dictionary
└── README.md


📊 Key Features

Automated ETL Pipeline: A master stored procedure orchestrates the data flow from Bronze to Gold.

Data Quality Checks: validation rules implemented in the Silver layer to flag inconsistencies.

Optimized Performance: Indexing and proper schema design for fast query execution.

👏 Acknowledgements & Inspiration

This project was built as a portfolio piece to demonstrate Data Engineering competencies.

It was heavily inspired by the amazing work of Baraa Salkini (DataWithBaraa). His tutorials and guidance on modern data warehousing concepts were instrumental in shaping the architecture and best practices applied here.

YouTube Channel: Data With Baraa

Original Concept: SQL Data Warehouse from Scratch
