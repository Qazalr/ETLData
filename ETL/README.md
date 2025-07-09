# 🧠 Databricks End-to-End Data Engineering Project

This project demonstrates a complete end-to-end data pipeline using modern data engineering tools including **Databricks Autoloader**, **Spark**, **Delta Live Tables**, **dbt**, and **Azure Synapse Analytics**.

---

## 🚀 Project Overview

The goal is to automate the process of ingesting, transforming, modeling, and loading data from CSV files to a warehouse for analytics and BI reporting.

---

## 📌 Technologies Used

| Tool | Purpose |
|------|---------|
| **Databricks Autoloader** | Automatically detects and ingests new files from a cloud storage folder |
| **Apache Spark** | Performs scalable, distributed data transformations |
| **Delta Live Tables (DLT)** | Orchestrates the ETL process using declarative pipeline logic |
| **dbt (Data Build Tool)** | Builds analytical models using SQL and organizes data into star schema |
| **Azure Synapse Analytics** | Stores final cleaned and transformed data for reporting and dashboarding |

---

## 🔁 Pipeline Architecture
[CSV Files]
⬇
[Autoloader (Bronze Layer)]
⬇
[Delta Live Tables (Silver Layer)]
⬇
[DLT (Gold Layer)]
⬇
[dbt Models → Star Schema]
⬇
[Azure Synapse Warehouse → Power BI / Analytics Tools]
---



## 📈 Features

- Fully automated ingestion using **Databricks Autoloader**
- Incremental data processing with **Delta Live Tables**
- Cleaned, transformed, and business-ready data in **Gold layer**
- Star schema modeling with **dbt**
- Final data pushed to **Azure Synapse** for reporting

---

## ✅ How to Run

1. Clone this repo in your Databricks workspace
2. Upload your CSVs into the monitored folder (e.g. `/mnt/raw`)
3. Run notebooks in order: `1_autoloader_ingestion` → `2_dlt_transformations` → `3_gold_layer_output`
4. Initialize and run dbt models to create final star schema tables
5. Connect Azure Synapse to Power BI or any analytics tool

---

## 📚 Learning Objectives

- Build scalable ETL pipelines using Spark & Delta Lake
- Understand how to structure data lakes using Bronze/Silver/Gold layers
- Learn how dbt simplifies data transformation and modeling
- Practice real-world data engineering workflows

---
