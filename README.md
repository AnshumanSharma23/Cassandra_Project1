# ETL Pipeline and Apache Cassandra Queries

## Overview
This project involves the implementation of an ETL (Extract, Transform, Load) pipeline for preprocessing event data files and executing Apache Cassandra queries to extract insights from the data. The goal is to transform raw event data into a format suitable for querying and analysis.

## Part I: ETL Pipeline for Pre-Processing
The ETL pipeline consists of the following steps:
1. **Data Extraction**: Original event CSV data files are processed to create a list of file paths.
2. **Data Transformation**: The data from each file is read and transformed into a unified format. Selected attributes are extracted and organized into rows.
3. **Data Loading**: The transformed data is written to a new CSV file that will serve as input for Apache Cassandra tables.

## Part II: Apache Cassandra Queries
After preprocessing the data, Apache Cassandra queries are designed to answer specific questions about the music app history. These questions include:
1. **Query 1**: Retrieve the artist, song title, and song length for a specific session ID and item in session.
2. **Query 2**: Obtain the artist, song (sorted by item in session), and user information (first and last name) for a given user ID and session ID.
3. **Query 3**: Identify every user who listened to a particular song.

## Conclusion
This project demonstrates the process of building an ETL pipeline for data preprocessing and executing Apache Cassandra queries to extract insights from the data. By combining data transformation and querying techniques, meaningful analysis of the music app history dataset can be achieved.
