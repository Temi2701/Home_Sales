# Home_Sales
Module 22 Challenge

## Overview
In this challenge, I utilised SparkSQL to analyse home sales data and derive key metrics. The tasks involved creating temporary views, partitioning data, caching and uncaching tables, and verifying table status. Below are the step-by-step instructions for the challenge.

## Instructions

### Import PySpark SQL Functions:
I imported the necessary PySpark SQL functions for the assignment.

### Read Data into Spark DataFrame:
I read the "home_sales_revised.csv" data into a Spark DataFrame.

### Create Temporary Table:
I created a temporary table named "home_sales."

### Answer SparkSQL Questions:
I utilised SparkSQL to answer the following questions:
Average price for a four-bedroom house sold each year (rounded to two decimal places).
Average price of a home for each year it was built with three bedrooms and three bathrooms (rounded to two decimal places).
Average price of a home for each year with three bedrooms, three bathrooms, two floors, and size greater than or equal to 2,000 sq. ft. (rounded to two decimal places).
"View" rating for homes costing more than or equal to $350,000 (including query runtime rounded to two decimal places).

### Cache Temporary Table:
I cached the "home_sales" temporary table.

### Check if Table is Cached:
I verified if the temporary table is successfully cached.

### Run Query on Cached Table:
I executed the query filtering out view ratings with an average price of $350,000 or more using the cached data.
I determined the runtime and compared it to the uncached runtime.

### Partition and Create Temporary Table for Parquet Data:
I partitioned the home sales dataset by the "date_built" field.
I read the formatted parquet data.
I created a temporary table for the parquet data.

### Run Query on Parquet Temporary Table:
I executed the query filtering out view ratings with an average price of $350,000 or more using the parquet temporary table.
I determined the runtime and compared it to the uncached runtime.

### Uncache Temporary Table:
I uncached the "home_sales" temporary table.

### Verify Uncaching:
I confirmed that the "home_sales" temporary table is successfully uncached using PySpark.
