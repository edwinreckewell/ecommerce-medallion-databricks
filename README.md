# Databricks Medallion Architecture: E-Commerce Data Pipeline

An end-to-end data engineering pipeline built on **Databricks**, **PySpark**, and **Delta Lake** using a Medallion Architecture (Bronze, Silver, Gold).

---

## 📌 Project Overview
This project processes e-commerce transactional data through three structured layers:
- **Bronze:** Raw data ingestion into immutable Delta tables with metadata tracking.
- **Silver:** Data cleaning, date parsing, deduplication, and PII masking.
- **Gold:** Aggregated business metrics, monthly revenue KPIs, and customer lifetime analysis.

---

## 📁 Repository Structure
```text
├── 01_bronze_ingestion.py        # Ingests raw data into Bronze Delta tables
├── 02_silver_transformations.py  # Cleans, parses, and masks sensitive data
├── 03_gold_aggregations.py       # Aggregates data into Gold business tables
└── README.md                     # Project documentation
