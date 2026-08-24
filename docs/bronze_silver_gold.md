# Bronze → Silver → Gold Pipeline

This document explains the multi-layer Delta Lake pipeline used in this project.

## Bronze Layer (Raw)
- Raw ingestion from CSV/JSON files
- Minimal transformations
- Schema inference
- Stored as Delta tables

## Silver Layer (Cleaned)
- Null handling
- Duplicate removal
- Schema enforcement
- Basic validation (row counts, referential checks)
- Standardized column names and formats

## Gold Layer (Curated)
- Business-ready tables
- Aggregations and joins
- Final QA checks
- Used for reporting, dashboards, or downstream consumption

## Why This Matters
This layered approach improves:
- Data quality
- Traceability
- Reproducibility
- Auditability

It is the standard pipeline design used in modern data engineering teams.
