# Project Architecture

This document explains the overall architecture of the Databricks Data QA Learning Project.

## 1. Databricks Workspace Setup
The project is built inside a Databricks workspace using:
- Databricks notebooks (Python, SQL, PySpark)
- DBFS/Volumes for raw file storage
- Delta Lake for managed tables
- Spark SQL for querying and validation

## 2. Storage Layout
Data is stored in the following layers:
- **Raw files** → DBFS/Volumes
- **Bronze tables** → Raw Delta tables
- **Silver tables** → Cleaned and validated Delta tables
- **Gold tables** → Curated business-ready tables

## 3. Pipeline Flow
1. Ingest raw CSV/JSON files into Bronze
2. Apply cleaning, schema enforcement, and validation in Silver
3. Produce curated Gold tables for downstream use

## 4. Validation Integration
Validation is performed using:
- SQL queries
- Python functions
- PySpark DataFrame API

This architecture mirrors real-world enterprise data engineering and QA pipelines.
