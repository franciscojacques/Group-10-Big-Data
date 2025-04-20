# BigData
This repository is accessible only by Group 10 and our prof

*PySpark Documentation*: https://spark.apache.org/docs/latest/api/python/user_guide/index.html
*Data Source Link*: https://catalog.data.gov/dataset/non-federal-acute-care-hospital-health-it-adoption-and-use


This project explores the adoption of Electronic Health Records (EHR) in non-federal acute care hospitals using big data tools. The analysis was conducted in a PySpark environment to efficiently handle, clean, and model the dataset at scale.

**Project Overview**

*Dataset*: U.S. Department of Health & Human Services — Non-Federal Acute Care Hospital Health IT Adoption

*Format*: CSV

*Objective*: Analyze adoption patterns using distributed processing and machine learning in PySpark

**Workflow Summary**
Data Import & Schema Update

Loaded CSV into Spark DataFrame

Renamed columns and updated schema types for consistency

Multimodel Imputation (PySpark MLlib + Custom Logic)

Built custom pipeline for handling missing values:

Used RandomForestRegressor and KNNImputer via PySpark integration

Performed group-based imputation (e.g., grouped by region/type)

Applied mean imputation as a fallback for remaining nulls

**Data Transformation**

Created a new Spark table after full imputation

Optimized schema for query efficiency

**SQL Queries**

Ran multiple exploratory queries via Spark SQL to derive insights


**Machine Learning Modeling**

Trained and compared multiple models (classification/regression where applicable):

Random Forest, Logistic Regression, and Gradient Boosted Trees using pyspark.ml

Evaluated model accuracy

**Visualization**

Visualized various aspects, including model accuracy differences

**Tech Stack**

Apache Spark (PySpark)

Spark MLlib

Spark SQL

Python 

Jupyter Notebooks / Databricks / VS Code

Git
