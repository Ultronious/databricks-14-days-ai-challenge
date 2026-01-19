🚀 Databricks 14 Days AI Challenge
Hands-on Data Engineering with Databricks, Spark & Delta Lake

This repository documents my day-wise learning journey (Day 1–11) through the Databricks 14 Days AI Challenge, focused on building strong fundamentals in data engineering, analytics, performance optimization, and ML preparation using Databricks.

The goal of this challenge is not just learning tools, but understanding how real-world data platforms are designed, optimized, and governed.

📌 What This Repository Covers

Distributed data processing with Apache Spark

Reliable data storage using Delta Lake

Medallion Architecture (Bronze → Silver → Gold)

Workflow orchestration with Databricks Jobs

Enterprise data governance with Unity Catalog (conceptual)

SQL analytics & dashboards

Performance optimization and tuning strategies

Statistical analysis & ML preparation

All implementations are done using Databricks Community Edition.

📓 Notebooks

Each day’s learning is implemented as Databricks notebooks, exported and versioned in this repository.

The notebooks combine theory + hands-on experimentation, closely resembling real-world data engineering workflows.

📅 Day-wise Learning Summary
📅 DAY 1 (09/01/2026) – Platform Setup & First Steps

📘 Key Learnings

Why Databricks is preferred over Pandas and Hadoop at scale

Introduction to the Lakehouse Architecture

Core Databricks workspace components:

Workspace

Compute

Data Explorer

How enterprises use Databricks for analytics and data engineering

Basics of PySpark DataFrames

🛠️ Hands-On Work

Set up Databricks Community Edition

Explored workspace navigation and cluster configuration

Created and executed the first Databricks notebook

Performed basic PySpark transformations

📅 DAY 2 (10/01/2026) – Apache Spark Fundamentals

📘 Key Learnings

Spark architecture: Driver, Executors, DAG

DataFrames vs RDDs

Lazy evaluation and execution flow

Transformations vs Actions

Databricks notebook magic commands (%python, %sql, %fs)

Reading and writing data using DBFS

🛠️ Hands-On Work

Ingested sample e-commerce CSV datasets

Loaded data into Spark DataFrames

Applied transformations:

select, filter, groupBy, orderBy

Exported processed results

📅 DAY 3 (11/01/2026) – PySpark Transformations Deep Dive

📘 Key Learnings

Distributed vs in-memory processing

Join strategies: Inner, Left, Right, Outer

Window functions for analytics

Aggregations and derived metrics

Pivot operations for funnel analysis

🛠️ Hands-On Work

Revenue analysis on transactional data

User behavior and engagement metrics

Conversion rate calculations

Exported transformed datasets

📅 DAY 4 (12/01/2026) – Delta Lake Introduction

📘 Key Learnings

Delta Lake architecture

ACID transactions in data lakes

Schema enforcement and validation

Delta Lake vs Parquet

🛠️ Hands-On Work

Converted raw CSV data into Delta format

Created Delta tables using PySpark and Spark SQL

Tested schema enforcement

Handled data quality issues

📅 DAY 5 (13/01/2026) – Delta Lake Advanced

📘 Key Learnings

Delta Lake Time Travel

MERGE operations for upserts

OPTIMIZE and ZORDER

VACUUM for storage cleanup

🛠️ Hands-On Work

Implemented incremental MERGE pipelines

Queried historical table versions

Optimized Delta tables

Cleaned obsolete files

📅 DAY 6 (14/01/2026) – Medallion Architecture

📘 Key Learnings

Bronze, Silver, and Gold layer responsibilities

Separation of concerns

Incremental processing patterns

Reliability with Delta Lake

🛠️ Hands-On Work

Designed a Medallion Architecture pipeline

Built:

Bronze (raw ingestion)

Silver (cleaning & validation)

Gold (business aggregations)

Practiced incremental updates

📅 DAY 7 (15/01/2026) – Workflows & Job Orchestration

📘 Key Learnings

Notebooks vs Jobs

Single-task vs multi-task workflows

Parameterization using widgets

Task dependencies and scheduling

Error handling in pipelines

🛠️ Hands-On Work

Parameterized notebooks using dbutils.widgets

Built a multi-task Databricks Job (Bronze → Silver → Gold)

Configured dependencies and scheduling

Implemented fail-fast error handling

🧠 Key Insight
Orchestration and scheduling are as important as transformations in production pipelines.

📅 DAY 8 (16/01/2026) – Unity Catalog & Data Governance

📘 Key Learnings

Enterprise data governance concepts

Unity Catalog hierarchy (Catalog → Schema → Table)

Managed vs external tables

Fine-grained access control

Data lineage and traceability

🛠️ Hands-On Work

Designed catalog and schema structure

Registered Delta tables across layers

Applied role-based permissions

Created governed views

🧠 Key Insight
Scalable data platforms require governance, ownership, and traceability.

📅 DAY 9 (17/01/2026) – SQL Analytics & Dashboards

📘 Key Learnings

Analytical Spark SQL queries

KPIs, trends, and ranking analysis

Chart selection for dashboards

🛠️ Hands-On Work

Built queries for:

Revenue trends

User funnels

Top products

Created KPI, line, and bar chart visualizations

Designed an interactive dashboard

🧠 Key Insight
Analytics is about clarity — asking the right questions and presenting answers effectively.

📅 DAY 10 (18/01/2026) – Performance Optimization

📘 Key Learnings

Query execution plans

Partitioning strategies

OPTIMIZE and ZORDER

Caching techniques

Benchmarking performance

🛠️ Hands-On Work

Analyzed execution plans

Applied partitioning

Optimized Delta tables

Benchmarked before vs after improvements

🧠 Key Insight
Performance optimization requires understanding execution behavior, not guesswork.

📅 DAY 11 (19/01/2026) – Statistical Analysis & ML Preparation

📘 Key Learnings

Descriptive statistics for data understanding

Hypothesis exploration (weekday vs weekend)

Correlation analysis

Feature engineering for ML

🛠️ Hands-On Work

Loaded curated Silver-layer data

Calculated statistical summaries

Explored behavioral hypotheses

Engineered ML-ready features:

Time-based features

Log-transformed price

Session-based behavior features

🧠 Key Insight
Machine learning starts with data understanding and feature quality, not models.

🏗️ High-Level Architecture & ML Flow
Raw Data
  ↓
Bronze (Raw Delta)
  ↓
Silver (Cleaned & Validated)
  ↓
Gold (Business Aggregates)
  ↓
SQL Analytics & Dashboards
  ↓
Statistical Analysis & Feature Engineering
  ↓
ML-Ready Datasets

This Lakehouse-based architecture enables data engineering, analytics, and ML to coexist on a single platform.

🧠 Key Takeaways (Day 1–11)

Spark enables scalable distributed processing

Databricks simplifies the full data lifecycle

Delta Lake ensures reliability and consistency

Medallion Architecture improves maintainability

Jobs enable production-grade workflows

Governance is critical at scale

Analytics, performance, and ML are tightly connected

🧰 Tech Stack

Apache Spark

PySpark

Spark SQL

Delta Lake

Databricks Jobs

Unity Catalog (conceptual)

Databricks Community Edition

🚀 What’s Next

Structured Streaming

Late-arriving data handling

Advanced performance tuning

Production-ready pipeline patterns

ML model integration

📂 Note on Repository Structure

Notebooks were developed directly in the Databricks workspace and exported here.
For learning purposes, Medallion Architecture is implemented within notebooks using logical sections rather than separate directories.
