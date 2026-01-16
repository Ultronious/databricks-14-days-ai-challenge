🚀 databricks-14-days-ai-challenge

Hands-on learning notes and Databricks notebooks from my Databricks 14 Days AI Challenge journey.
This repository captures my day-wise progression in data engineering, combining core theory, practical PySpark implementations, and real-world data lake concepts using Databricks.

📓 Notebooks
Each day’s hands-on work is implemented in Databricks notebooks within this repository.

📅 DAY 1 (09/01/2026) – Platform Setup & First Steps
📘 Key Learnings

Why Databricks is better suited than Pandas and Hadoop for large-scale data processing

Fundamentals of the Lakehouse architecture

Core Databricks workspace components:

Workspace

Compute

Data Explorer

How enterprises use Databricks for analytics and data engineering

Executed first PySpark DataFrame operations

🛠️ Hands-On Work

Set up Databricks Community Edition

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

Delta Lake architecture and core concepts

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

📅 DAY 6 (14/01/2026) – Medallion Architecture
📘 Key Learnings

Understanding the Medallion Architecture in production-grade data platforms

Role of each layer:

Bronze: Raw, ingested data with minimal transformation

Silver: Cleaned, validated, and structured data

Gold: Aggregated, business-ready datasets

Best practices for separation of concerns

Incremental processing patterns to avoid full reprocessing

How Delta Lake supports reliability and traceability

🛠️ Hands-On Work

Designed a three-layer Medallion architecture using Delta tables

Built Bronze layer for raw data ingestion

Implemented Silver layer with:

Data cleaning

Schema validation

Basic transformations

Created Gold layer with business-level aggregations

Practiced incremental updates across layers

📅 DAY 7 (15/01/2026) – Workflows & Job Orchestration
📘 Key Learnings

Difference between Databricks Notebooks and Jobs

Why notebooks are suited for development while Jobs handle production execution

Single-task vs multi-task workflows

Parameterization using Databricks widgets

Task dependencies and execution order

Scheduling and retry behavior in Databricks Jobs

Importance of explicit error handling in automated pipelines

🛠️ Hands-On Work

Parameterized notebooks using dbutils.widgets for dynamic execution

Designed a multi-task Databricks Job following the Medallion pattern:

Bronze → Silver → Gold

Configured task dependencies to enforce correct execution order

Scheduled automated workflow execution

Implemented fail-fast error handling for visibility and reliability

🧠 Key Insight

Moving from manual notebook execution to Jobs highlighted how orchestration, dependencies, and scheduling are just as important as transformation logic when building reliable pipelines.

📅 DAY 8 (16/01/2026) – Unity Catalog & Data Governance
📘 Key Learnings

Enterprise data governance concepts in Databricks

Unity Catalog hierarchy:

Catalog → Schema → Table

Differences between managed and external Delta tables

Fine-grained access control using GRANT and REVOKE

How data lineage enables pipeline traceability

Using views to expose curated datasets while protecting raw data

🛠️ Hands-On Work

Designed catalog and schema structure aligned with Bronze, Silver, and Gold layers

Registered Delta tables across pipeline layers

Applied role-based permissions for engineers and analysts

Created governed views for controlled business access

Studied how Unity Catalog centralizes governance without slowing analytics

🧠 Key Insight

Scalable data platforms require more than pipelines—they need governance, ownership, and traceability. Unity Catalog brings structure and accountability at enterprise scale.

🧠 Key Takeaways (Day 1–8)

Apache Spark enables scalable distributed processing beyond in-memory tools

Databricks simplifies the full lifecycle of data engineering

Delta Lake ensures reliability through ACID transactions and schema enforcement

Medallion Architecture improves pipeline clarity and maintainability

Databricks Jobs enable production-grade workflow orchestration

Unity Catalog is essential for enterprise governance, security, and lineage

Learning by building, breaking, and fixing pipelines reinforces real-world understanding

🧰 Tech Stack

Apache Spark

PySpark

Delta Lake

Spark SQL

Databricks Jobs

Unity Catalog (conceptual)

Databricks Community Edition

🚀 Upcoming Topics

Structured Streaming with Apache Spark

Handling late-arriving and incremental data

Performance tuning and optimization strategies

Production-ready pipeline design patterns

Applying governance and orchestration to real-world use cases

📂 Note on Repository Structure

The notebooks in this repository were developed and exported directly from the Databricks workspace.
For learning purposes, Medallion Architecture (Bronze, Silver, Gold) is implemented within notebooks using logical sections rather than separate directories.
