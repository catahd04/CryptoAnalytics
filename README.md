
CryptoScope 📊
Cryptocurrency Analytics Engineering Platform

📌 Overview

CryptoScope is an end-to-end Analytics Engineering project designed to ingest, transform, and model cryptocurrency data for analytical purposes.

The project leverages AWS S3 as the data source, Snowflake as the cloud data warehouse, and dbt (Data Build Tool) for data transformation and modeling.

The platform processes cryptocurrency datasets, including Bitcoin (BTC) and Ethereum (ETH), transforming raw data into structured, analytics-ready models to support market analysis and data-driven insights.

🏗️ Architecture

The project follows a modern data architecture based on cloud storage, data warehousing, and transformation technologies.

Data Pipeline:
Data Source – AWS S3: Cryptocurrency datasets are stored in S3 buckets.
Automated Data Ingestion – Snowflake: Snowflake integrates with AWS S3 to automatically ingest new data files into the data warehouse.
Raw Data Layer: Ingested data is stored in Snowflake as raw datasets.
Data Transformation – dbt: dbt processes raw data using SQL-based transformations.
Incremental Modeling: Incremental dbt models process new and updated records instead of rebuilding entire datasets.
Analytics Layer: Final data models provide structured datasets ready for analytical queries and reporting.

🛠️ Tech Stack
Technology	Purpose
AWS S3	Raw cryptocurrency data storage
Snowflake	Cloud Data Warehouse
dbt	Data transformation and modeling
SQL	Data transformation logic
Git & GitHub	Version control

📂 Project Structure

CryptoScope/
│
├── analyses/          # Analytical SQL queries
├── macros/            # Reusable dbt macros
├── models/
│   ├── staging/       # Initial data transformations
│   ├── intermediate/  # Business logic and transformations
│   └── marts/         # Final analytical models
│
├── seeds/             # Static reference datasets
├── snapshots/         # Historical data tracking
├── tests/             # Data quality tests
├── dbt_project.yml    # dbt project configuration
└── README.md

🔄 Data Workflow

AWS S3 Buckets
      |
      v
 Cryptocurrency Data
  (BTC / ETH)
      |
      v
   Snowflake
   (Raw Layer)
      |
      v
      dbt
  (Transformations)
      |
      v
  Staging Models
      |
      v
Intermediate Models
      |
      v
   Marts Layer
      |
      v
Analytics & Insights

🎯 Project Objectives
Build an end-to-end data pipeline for cryptocurrency datasets.
Implement data transformations using dbt and SQL.
Design scalable and maintainable data models.
Leverage Snowflake for cloud-based data warehousing.
Apply data quality testing and transformation best practices.
Prepare structured datasets for cryptocurrency market analysis.
🚀 Getting Started
Prerequisites
Snowflake account.
AWS S3 access.
dbt Core or dbt Cloud.
Python environment.
Setup
Clone the repository.
Configure your Snowflake connection.
Configure AWS S3 access and storage integration.
Install the required dbt dependencies.
Execute dbt commands to build the data models.
bash
dbt deps
dbt debug
dbt run
dbt test

📈 Future Improvements

Integrate BI tools for data visualization.

👨‍💻 Authora> Catalina Herrera

Developed as a Analytics Engineering project focused on modern data stack technologies and cryptocurrency analytics.
