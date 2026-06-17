# PySpark Databricks Learning

Step-by-step PySpark learning using the BigMart Sales dataset on Databricks.

This is an active learning repository — updated as I progress through new topics.

## What's Covered (as of June 2026)

- **Data Ingestion** — Reading CSV and JSON files into Spark DataFrames
- **Schema Definition** — Inferred schema, DDL string schema, StructType explicit schema
- **Column Operations** — select(), alias(), withColumnRenamed(), withColumn(), lit()
- **Filtering** — Single conditions, AND/OR logic, isNull(), isin()
- **String Manipulation** — regexp_replace() for data standardization
- **Type Casting** — Casting between StringType, DoubleType, IntegerType
- **Sorting** — sort() and orderBy() in ascending and descending order
- **GroupBy & Aggregations** — groupBy() with count(), sum(), avg(), min(), max()

## In Progress / Coming Next

- Joins (inner, left, right, outer)
- Window Functions
- Spark SQL
- Delta Lake basics

## Dataset

BigMart Sales dataset — retail transaction data with product and outlet information.
Source: [Analytics Vidhya BigMart Sales](https://datahack.analyticsvidhya.com/contest/practice-problem-bigmart-sales-prediction/)

Data files are not included in this repo due to size. Download from the source above and place in the `data/` folder.

## Environment

- Apache PySpark
- Databricks (Community Edition compatible)
- Python 3.x

## How to Use

1. Download the dataset and upload to Databricks DBFS at `/FileStore/tables/`
2. Import the notebook from the `notebooks/` folder into your Databricks workspace
3. Run cells sequentially

## Status

🟡 In progress — actively adding new topics
