# -IPL-Data-Analysis-using-PySpark-Snowflake-

🏏 IPL Data Analysis using PySpark & Snowflake
This project is a Big Data analytics pipeline for analyzing Indian Premier League (IPL) cricket data using Apache Spark, PySpark, and Snowflake. It performs ETL (Extract, Transform, Load) operations on cricket data stored in HDFS, processes and analyzes it using PySpark, and finally loads the cleaned and enriched data into Snowflake, a cloud data warehouse.

⚙️ Technologies Used
Apache Spark (PySpark)

HDFS (Hadoop Distributed File System)

Snowflake (via JDBC connector)

Python

Spark SQL & Window Functions

📊 Key Features
🧹 ETL Pipeline
Defined custom schemas for all datasets

Loaded raw datasets from HDFS

Applied data cleaning, normalization, and missing value handling

Enriched data with aggregations, window functions, and derived columns

Loaded the final transformed data into Snowflake using Spark-Snowflake connector

🏏 Cricket Data Analysis
Ball-by-Ball Analysis
Removed invalid deliveries (wides, no-balls)

Calculated total & average runs per match and innings

Applied window functions for running totals

Flagged high-impact balls

Match Analysis
Extracted year, month, day from match dates

Categorized win margins

Analyzed correlation between toss and match wins

Player Analysis
Cleaned and standardized player names

Categorized players by batting hand

Labeled veteran players (age ≥ 35)

Calculated years since debut

☁️ Snowflake Integration
Used the Spark-Snowflake connector to write transformed DataFrames to Snowflake

Configured Snowflake connection with .config("spark.jars.packages", ...) setup

Enables scalable, secure, and query-optimized cloud storage for post-processing and reporting
