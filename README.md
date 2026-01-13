🚀 databricks-14-days-ai-challenge

Hands-on learning notes and Databricks notebooks from my Databricks 14 Days AI Challenge journey.
This repository showcases my day-wise progression in data engineering, combining core theory, practical PySpark implementations, and real-world data lake concepts using Databricks.

📓 Notebooks: Each day’s hands-on work is implemented in Databricks notebooks within this repository.

📅 DAY 1 (09/01/2026) – Platform Setup & First Steps
📘 Key Learnings

Why Databricks outperforms Pandas and Hadoop for large-scale data processing

Fundamentals of the Lakehouse architecture

Core Databricks workspace components:

Workspace

Compute

Data Explorer

How enterprises use Databricks for analytics and data engineering

Executed first PySpark DataFrame operations

🛠️ Hands-On Work

Set up Databricks Community Edition environment

Explored workspace navigation and cluster configuration

Created and executed the first Databricks notebook

Performed basic PySpark transformations

📅 DAY 2 (10/01/2026) – Apache Spark Fundamentals
📘 Key Learnings

Apache Spark architecture: Driver, Executors, DAG

DataFrames vs RDDs

Lazy evaluation and execution flow

Transformations vs Actions

Databricks notebook magic commands (%python, %sql, %fs)

Reading and writing data using DBFS

🛠️ Hands-On Work

Ingested sample e-commerce CSV datasets

Loaded data into Spark DataFrames

Applied core transformations:

select

filter

groupBy

orderBy

Exported processed results for downstream use

📅 DAY 3 (11/01/2026) – PySpark Transformations Deep Dive
📘 Key Learnings

Differences between distributed processing (PySpark) and in-memory processing (Pandas)

Join strategies: Inner, Left, Right, Outer

Window functions for analytical use cases

Aggregations and derived metric creation

Pivot operations for funnel and conversion analysis

🛠️ Hands-On Work

Performed revenue analysis on transactional data

Implemented user behavior and engagement metrics

Calculated conversion rates using advanced transformations

Exported transformed datasets for reporting

📅 DAY 4 (12/01/2026) – Delta Lake Introduction
📘 Key Learnings

Delta Lake architecture and fundamentals

ACID transactions in data lakes

Schema enforcement and validation

Comparison of Delta Lake vs Parquet

🛠️ Hands-On Work

Converted raw CSV data into Delta format

Created Delta tables using PySpark and Spark SQL

Tested schema enforcement to prevent invalid writes

Handled data quality issues during ingestion

📅 DAY 5 (13/01/2026) – Delta Lake Advanced
📘 Key Learnings

Delta Lake Time Travel using version history

MERGE operations for incremental upserts

Table optimization using OPTIMIZE

Data skipping using ZORDER

Storage cleanup and cost management using VACUUM

🛠️ Hands-On Work

Implemented incremental MERGE pipelines

Queried historical versions of Delta tables

Optimized Delta tables for query performance

Cleaned obsolete files to manage storage efficiently

🧠 Key Takeaways

Apache Spark enables scalable distributed data processing

Databricks simplifies end-to-end data engineering workflows

Delta Lake makes data lakes reliable, auditable, and production-ready

Optimization and versioning are essential for real-world data pipelines

🧰 Tech Stack

Apache Spark

PySpark

Delta Lake

Spark SQL

Databricks Community Edition

🚀 Upcoming Topics

Structured Streaming with Spark

Performance tuning and optimization

End-to-end data pipeline design

Real-world data engineering projects
