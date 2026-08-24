# Data Quality Rules

This document lists the data quality checks implemented in this project.

## 1. Row Count Checks
Ensures expected number of records are present after ingestion and transformation.

## 2. Null Checks
Identifies missing values in critical fields such as IDs, names, or keys.

## 3. Duplicate Checks
Detects duplicate rows based on primary keys or business keys.

## 4. Schema Validation
Verifies column names, data types, and structure match expected schema.

## 5. Referential Integrity
Ensures relationships between tables are valid (e.g., product_id exists in product catalog).

## 6. Reconciliation
Compares source vs target tables to ensure transformations did not lose or alter data incorrectly.

## 7. Business Rule Validation
Checks domain-specific rules such as:
- price > 0
- quantity >= 1
- valid email formats

These rules form the foundation of a QA/Test Architect’s validation framework.
