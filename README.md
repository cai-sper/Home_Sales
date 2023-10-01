# Home Sales Analysis with PySpark and SparkSQL

## Overview

This project employs PySpark and SparkSQL to analyze home sales data. The analysis aims to uncover key metrics associated with home prices based on various features, such as the number of bedrooms, bathrooms, and view ratings.

## Table of Contents

1. [Features](#features)
2. [Code and Steps](#code-and-steps)
3. [Performance Metrics](#performance-metrics)

## Features

- Import home sales data into a Spark DataFrame
- Create and manage temporary tables for faster query execution
- Compute average home prices based on different features

## Code and Steps

The project takes the following steps:

1. Import the necessary PySpark SQL functions
2. Read the `home_sales_revised.csv` data into a Spark DataFrame
3. Create a temporary table named `home_sales`
4. Execute various SparkSQL queries to answer specific questions about home prices
5. Cache and uncache the temporary table to compare performance

## Performance Metrics

- The cached runtime was 0.15 seconds faster than the uncached runtime. This improvement is likely because caching loads the data into memory, making subsequent operations more efficient.
- The Parquet runtime was approximately 0.12 seconds faster than the cached version. This could be due to Parquet's optimized columnar storage format, which allows for quicker read operations.