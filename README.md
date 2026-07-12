# PySpark Essentials Practice

A hands-on practice notebook for learning core PySpark and Databricks mechanics — reading nested JSON, filtering, `explode`, flattening nested structs, joins, lazy evaluation (`.explain()`), and writing Delta tables.

## Purpose

Built as prep work before tackling a real healthcare data pipeline (Synthea FHIR data). The dataset here is a simplified, FHIR-like toy schema — customers and orders with nested arrays and cross-record references — designed to mirror FHIR's structural challenges (nested objects, arrays, reference strings) without the added complexity of healthcare-specific concepts. The goal was to build confidence with PySpark fundamentals in isolation before combining them with FHIR's domain complexity and AWS Glue's additional abstractions.

## Contents

- `pyspark_essentials_practice.ipynb` — the notebook, runnable in any PySpark environment
- `pyspark_essentials_practice.html` — a static, viewable export of the notebook with outputs, no Spark environment required

## Skills Practiced

- Reading and inspecting nested JSON schemas
- Filtering mixed record types from a single source
- Flattening nested structs and exploding arrays
- Parsing reference-style foreign keys (`"Customer/cust-001"`)
- Joins and data validation checks
- Lazy evaluation and query plans
- Writing results as Delta tables
