# PySpark Databricks Learning

PySpark fundamentals on Databricks using the BigMart Sales dataset.

This is an active learning repo — updated as I cover new topics.

---

## Topics Covered

### Data Ingestion
- Reading JSON files with `spark.read.json()`
- Reading CSV files with `spark.read.csv()` using `inferSchema` and `header` options
- Exploring files with `dbutils.fs.ls()`

### Schema Definition
- Inferred schema via `inferSchema=True`
- Explicit DDL string schema

### DataFrame Operations
- `select()` with `col()`
- `alias()` for column renaming within select
- `withColumnRenamed()` to rename existing columns
- `display()` and `printSchema()` for inspection

### Filtering
- Single condition: `col == value`
- Multiple conditions with `&` (AND) and `|` (OR)
- Null checks with `isNull()`

### Column Transformations
- `withColumn()` to add new columns
- `lit()` for literal/constant values
- Arithmetic operations between columns
- Type casting with `.cast("double")`

---

## In Progress / Coming Next

- regexp_replace() for string standardization
- sort() and orderBy()
- GroupBy and aggregations
- Joins
- Window Functions
- Spark SQL

---

## Dataset

BigMart Sales — retail transaction data with product and outlet information.

Download: [Analytics Vidhya BigMart Sales](https://datahack.analyticsvidhya.com/contest/practice-problem-bigmart-sales-prediction/)

Upload to Databricks at: `/Volumes/dbacademy/default/tutorials/`

## Environment

- PySpark on Databricks
- Python 3.x
- Unity Catalog (Volumes-based file path)

## Status

🟡 Work in progress
