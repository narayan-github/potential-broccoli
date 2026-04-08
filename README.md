# 🏥 Healthcare Patient Records Pipeline (Databricks Lakehouse)

This project implements an end-to-end healthcare data pipeline using the Databricks Lakehouse architecture (Bronze → Silver → Gold) with a strong focus on data governance, scalability, and real-time processing.

The pipeline ingests patient visit, demographic, and billing data, transforms it into enriched analytical datasets, and produces clinical and financial KPIs while ensuring HIPAA-aligned data protection using Unity Catalog.

---

## 🚀 Key Features

- **Medallion Architecture**
  - Bronze: Raw ingestion with schema enforcement & constraints
  - Silver: Cleaned, enriched, and joined datasets
  - Gold: Business-level KPIs and analytics

- **Data Engineering**
  - PySpark transformations
  - Delta Lake (ACID, Time Travel, CDF)
  - Incremental ingestion using Auto Loader

- **Advanced Modeling**
  - SCD Type 2 for patient demographics
  - Visit categorization (long/short/day stay)
  - Financial metrics (billing, insurance, liability)

- **Streaming Pipeline**
  - Structured Streaming with watermarking
  - Real-time patient admissions processing
  - Fault-tolerant with checkpointing

- **Workflow Orchestration**
  - Databricks Workflows (job scheduling, retries, dependencies)

- **Governance & Security (HIPAA-aligned)**
  - Unity Catalog integration
  - Column-level masking (PII protection)
  - Row-level access control

---

## 🧱 Tech Stack

- Databricks Lakehouse
- PySpark
- Delta Lake
- Databricks SQL
- Unity Catalog
- Structured Streaming

---

## 📊 Outputs

- Enriched patient-level dataset (Silver)
- Department-level clinical KPIs (Gold)
- Monthly financial analytics
- Real-time admissions table
- Secure, governed data access layer

---

## 📌 Use Case

Designed for healthcare systems processing large-scale patient records requiring:
- Regulatory compliance (HIPAA)
- Real-time data ingestion
- Reliable analytics and reporting
