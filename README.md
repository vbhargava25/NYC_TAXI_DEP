###End-to-End Data Pipeline for NYC Taxi Trip Analysis Using Azure Databricks

![img alt](https://github.com/vbhargava25/NYC_TAXI_DEP/blob/main/cf.png?raw=true)

🛠️ Step-by-Step Pipeline
1. 📂 Data Understanding
Explored the schema, types, and business value of the NYC Taxi dataset.

2. 🔧 Azure Databricks Setup
Created a Databricks Workspace and launched compute clusters for ETL workloads.

3. 🔐 Secure Data Access
Configured Azure Active Directory Service Principal for secure authentication.

Granted appropriate read/write permissions to Azure Data Lake Storage (ADLS).

4. 🔗 Lakehouse Integration
Used credential passthrough to authenticate Databricks access to ADLS.

Verified data visibility and structure within the data lake.

5. 🥉 Bronze Layer – Raw Ingestion
Ingested raw CSV/Parquet files using PySpark.

Stored as-is in the Bronze layer for traceability.

6. 🥈 Silver Layer – Cleaning & Transformation
Applied schema enforcement and column renaming.

Removed invalid records (e.g., zero fare, zero distance).

Extracted useful time-based features (year, month).

Stored transformed data as Parquet files.

7. 🥇 Gold Layer – Aggregations & Delta Tables
Created Delta Tables for analytics (e.g., trips per day, avg fare by zone).

Enabled time-travel and efficient querying.

8. ⚙️ Automation
Built and scheduled Databricks Jobs to update the pipeline daily.

9. 📈 Analytics & Reporting
Queried Delta Tables using SQL within Databricks.

Connected to Power BI to build interactive dashboards for insights.

✅ What We Achieved
🚀 Implemented a modular, scalable data lakehouse pipeline.

🔁 Ensured automated, secure, and versioned data workflows.

📉 Delivered actionable business insights through dashboards

ink used https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page
