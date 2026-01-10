# AWS Batch Data Engineering Pipeline

## 📌 Project Overview
This project demonstrates an end-to-end **batch data engineering pipeline on AWS**, built from scratch to understand how real-world data platforms are designed and implemented.

The pipeline ingests raw data into an Amazon S3 data lake, processes it using Apache Spark on EMR, generates analytics-ready metrics, and loads them into Amazon Redshift for visualization.

---

## 🏗️ Architecture Overview

**Data Flow:**

1. Raw CSV data is ingested into Amazon S3
2. Data is stored in a structured data lake (`raw`, `clean`, `analytics`)
3. Apache Spark on EMR processes and transforms the data
4. Metrics are generated using DuckDB
5. Final analytics data is loaded into Amazon Redshift
6. Dashboards are created using Amazon QuickSight
7. The entire pipeline is orchestrated using Apache Airflow running on EC2

---

## 🧰 Technologies Used

- Amazon S3 (Data Lake)
- Apache Airflow (EC2)
- Amazon EMR (Apache Spark)
- DuckDB
- Amazon Redshift
- Amazon QuickSight
- GitHub (Version Control)

---

## 📂 Data Lake Structure

```text
s3://de-batch-data-lake-prakash/
├── raw/
│   ├── csv/
│   └── db/
├── clean/
└── analytics/
