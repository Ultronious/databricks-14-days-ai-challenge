# databricks-14-days-ai-challenge
Hands-on learning notes and notebooks from my Databricks learning journey.
### **DAY 1 (09/01/26)– Platform Setup & First Steps**
📅 09/01/2026

## What I learned
- Why Databricks is preferred over Pandas and Hadoop for large-scale data
- Basics of Lakehouse architecture
- Databricks workspace components (Workspace, Compute, Data Explorer)
- How Databricks is used by companies for large-scale analytics
- Ran my first PySpark commands

## What I worked on
- Created a Databricks Community Edition account
- Explored workspace navigation and compute setup
- Created my first Databricks notebook
- Executed basic PySpark DataFrame operations

### 📓 Notebooks
- notebooks/day1_databricks_basics.ipynb
  
## Practice
```python
data = [("iPhone", 999), ("Samsung", 799), ("MacBook", 1299)]
df = spark.createDataFrame(data, ["product", "price"])
df.show()

df.filter(df.price > 1000).show()
```
### **DAY 2 (10/01/26) – Apache Spark Fundamentals**
📅 10/01/2026

🚀 Spark Fundamentals & Databricks Hands-On

This repository documents my learning journey of Apache Spark fundamentals, focusing on core concepts, architecture, and hands-on DataFrame operations using Databricks notebooks.

It includes concise theory notes, practical tasks, and a PDF reference suitable for revision and interviews.

📘 What I Learned
🔹 Spark Core Concepts

Spark architecture: Driver, Executors, DAG

Difference between DataFrames and RDDs

Lazy evaluation and execution flow

Spark actions vs transformations

🔹 Databricks Essentials

Notebook magic commands:

%python

%sql

%fs

Reading and writing data using DBFS

Running Spark SQL on DataFrames

🛠️ Hands-On Tasks Completed

Uploaded a sample e-commerce CSV dataset

Read data into a Spark DataFrame

Performed core operations:

select

filter

groupBy

orderBy

Exported processed results back to storage

