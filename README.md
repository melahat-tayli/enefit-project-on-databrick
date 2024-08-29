# BUILDING ROBUST DATA PIPELINES WITH MEDALLION ARCHITECTURE

The purpose of this project is to develop a robust data pipeline capable of accurately predicting Estonia's electricity consumption and production. 

The data used in this project is multidimensional, encompassing various factors such as gas and electricity prices, weather forecasts, and historical weather data. This data is distributed across eight separate files and requires careful merging. While some files contain hourly data points, others offer only daily data. Following a thorough exploratory data analysis (EDA), I created new data features to combine these files into meaningful tables for dashboards and machine learning analysis.

-This project was implemented on databricks platform. Databricks is a great platform for ETL pipelines, dashboards, visualizations and machine learning modellings.

-In this project, I used pyspark for data loading, cleaning, merging and table creation purposes.

-I used spark sql for creating a database. I chose medallion architecure for building data pipelines (bronze tables for raw data ingestion, silver tables for cleaned data and gold tables for merged data for machine learning applications)

-Updated data is inserted to tables using slowly changing dimension 1 data modelling technique.

