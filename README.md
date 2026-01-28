## 📌 Project Overview

This project demonstrates an **end-to-end cloud data engineering pipeline** built using **Azure Data Factory (ADF)** and **Azure Databricks**. The pipeline ingests raw data from an external source, performs scalable data transformations using **Databricks (Apache Spark)**, and loads curated data into an **Azure SQL Database** for analytics and reporting.

This repository showcases hands-on experience in:

* ETL pipeline orchestration using Azure Data Factory
* Big data processing with Azure Databricks
* Parameterized, scalable, and production-ready pipelines
* Cloud-based data engineering best practices

---

## Architecture

**Source(GitHub) → Azure Data Factory → Azure Databricks → Azure SQL Database**

* **Source**: HTTP / API / CSV files
* **Orchestration**: Azure Data Factory
* **Transformation**: Azure Databricks (PySpark)
* **Sink**: Azure SQL Database

---

## ☁️ Azure Resources Used

* **Resource Group**: `abhiresource`
* **Azure Data Factory**: `Consoleabhidf`
* **Azure Databricks Workspace**
* **Azure SQL Server**: `consoleserver.database.windows.net`
* **Azure SQL Database**: `abhidatabase`

---

## 🔐 Authentication & Security

* Azure SQL Authentication / Microsoft Entra Authentication
* Secure linked services in Azure Data Factory
* Databricks workspace access via Azure-managed identity

---

## 🔄 Pipeline Workflow

### 1️⃣ Data Ingestion (Azure Data Factory)

* Create ADF pipeline with **Copy Data activity**
* Source configured using **HTTP Linked Service**
* Parameterized datasets for dynamic file ingestion
* Raw data staged for processing

### 2️⃣ Data Transformation (Azure Databricks)

* Databricks notebook triggered from ADF
* Data cleaned, transformed, and enriched using **PySpark**
* Business rules applied (null handling, type casting, aggregations)

Example operations:

* Data cleansing
* Schema validation
* Aggregations & joins

### 3️⃣ Data Loading (Azure SQL Database)

* Transformed data written to Azure SQL tables
* Optimized schema for analytics and reporting
* Supports incremental and full loads

---

## ⚙️ Key Features

* End-to-end ETL orchestration
* Parameterized ADF pipelines
* Scalable Spark-based transformations
* Secure Azure SQL integration
* Modular and reusable pipeline design

---

## 🧪 Testing & Validation

* Verified successful ingestion from source
* Validated Databricks transformations
* Confirmed row counts and schema accuracy in Azure SQL

---

## 📂 Repository Structure

```
├── adf_pipelines/
│   └── copy_and_transform_pipeline.json
├── databricks_notebooks/
│   └── data_transformation.py
├── datasets/
│   ├── http_dataset.json
│   └── sql_dataset.json
├── linkedServices/
│   ├── http_linked_service.json
│   ├── databricks_linked_service.json
│   └── sql_linked_service.json
├── README.md
```

---

## 🚀 How to Run

1. Deploy Azure resources (ADF, Databricks, SQL)
2. Import pipelines and notebooks
3. Configure linked service credentials
4. Trigger the ADF pipeline manually or via schedule

---

##  Skills Demonstrated

* Azure Data Factory
* Azure Databricks (PySpark)
* Big Data Processing
* ETL / ELT Pipelines
* Cloud Data Engineering
* Delta Lake implementation
* Data quality checks
* CI/CD for ADF pipelines

---

## 📌 Future Enhancements
* Power BI integration for reporting

---

## 👤 Author

**Abhishek Kumar**
Data Analyst | Data Engineer | Python | SQL | Azure | Databricks

---

