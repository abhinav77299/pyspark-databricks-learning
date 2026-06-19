# PySpark Databricks Learning

PySpark fundamentals on Databricks using the BigMart Sales dataset.

This is an active learning repo — updated as I cover new topics.

---

## Topics Covered

### Day 1 — Foundations

**Data Ingestion**
- Reading JSON files with `spark.read.json()`
- Reading CSV files with `spark.read.csv()` using `inferSchema` and `header` options
- Exploring files with `dbutils.fs.ls()`

**Schema Definition**
- Inferred schema via `inferSchema=True`
- Explicit DDL string schema

**DataFrame Operations**
- `select()` with `col()`
- `alias()` for column renaming within select
- `withColumnRenamed()` to rename existing columns
- `display()` and `printSchema()` for inspection

**Filtering**
- Single condition: `col == value`
- Multiple conditions with `&` (AND) and `|` (OR)
- Null checks with `isNull()`

**Column Transformations**
- `withColumn()` to add new columns
- `lit()` for literal/constant values
- Arithmetic operations between columns
- Type casting with `.cast()`

### Day 2 — Sorting, Cleaning, Dates, Aggregations

**Sorting & Filtering**
- `sort()` with single and multiple columns, ascending/descending
- `limit()` to restrict row count
- `drop()` to remove columns
- `dropDuplicates()` on subset of columns

**Union Operations**
- `union()` to combine DataFrames with matching schema
- Schema mismatch behavior when unioning DataFrames

**Date Functions**
- `current_date()`
- `date_add()` and `date_sub()`
- `datediff()` between two date columns

**Handling Nulls**
- `dropna("all")` and `dropna("any")`
- `dropna(subset=[...])` for targeted null removal
- `fillna()` with constant values and per-column fill

**String Operations**
- `split()` to break strings into arrays
- Indexing into split array columns

**Aggregations**
- `groupBy()` with `.sum()`
- `groupBy()` with `.agg()` and `alias()`
- `collect_list()` to aggregate values into arrays per group

---

## In Progress / Coming Next

- Joins
- Window Functions
- Spark SQL
- Delta Lake basics

---

## Dataset

BigMart Sales — retail transaction data with product and outlet information.

Download: [Analytics Vidhya BigMart Sales](https://datahack.analyticsvidhya.com/contest/practice-problem-bigmart-sales-prediction/)

Upload to Databricks at: `/Volumes/dbacademy/default/tutorials/`

## Environment

- PySpark on Databricks
- Python 3.x
- Unity Catalog (Volumes-based file path)

## Notebooks

| File | Topics |
|---|---|
| `PySpark_DataProcessing1.ipynb` | Day 1 — Ingestion, schema, filtering, column transformations |
| `PySpark_DataProcessing2.ipynb` | Day 2 — Sorting, nulls, dates, string ops, aggregations |

## Status

🟡 Work in progress
