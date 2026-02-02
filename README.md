# data_modeling
Built an ETL pipeline in Python to preprocess and denormalize raw music streaming event data, 
then designed and implemented a query-driven data model in Apache Cassandra. 
Created optimized tables based on specific access patterns, using appropriate partition and 
clustering keys to enable efficient, scalable reads without joins or filtering.

# ETL Pipeline with Apache Cassandra

## Project Overview
This project implements an end-to-end **ETL pipeline** and **NoSQL data model** using **Apache Cassandra** for a music streaming application. Raw event data is processed, denormalized, and stored in Cassandra tables designed specifically for predefined query patterns.

## Project Goals
- Process and clean raw CSV event data
- Design Cassandra tables based on query requirements
- Execute efficient queries using appropriate partition and clustering keys
- Demonstrate NoSQL data modeling best practices

## What This Project Does
- Parses multiple raw CSV files and combines them into a single denormalized dataset
- Creates a Cassandra keyspace and query-optimized tables
- Loads transformed data into Cassandra
- Runs predefined queries to validate the data model

## Queries Supported
1. Retrieve artist, song title, and song length by session ID and item number  
2. Retrieve song listening history for a given user and session, ordered by item number  
3. Retrieve all users who listened to a specific song  

## Technologies Used
- Python
- Apache Cassandra
- CQL (Cassandra Query Language)
- Jupyter Notebook
- CSV data processing

## How to Run
1. Start a local Cassandra instance  
2. Open the Jupyter Notebook  
3. Run all cells in order to:
   - Create tables
   - Load data
   - Execute queries

## Key Concepts Demonstrated
- Query-driven NoSQL data modeling
- Denormalization for performance
- Partition keys and clustering columns
- Efficient reads without joins or filtering

## Outcome
This project demonstrates how to design scalable and high-performance data models in Apache Cassandra by modeling data around access patterns rather than entities.
