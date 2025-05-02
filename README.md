# Serverless Data Lake on AWS with Glue, Athena, and QuickSight

This project demonstrates how to build a serverless data lake architecture using AWS services including Amazon S3, AWS Glue, Amazon Athena, and Amazon QuickSight. It provides an end-to-end pipeline for data ingestion, ETL processing, query execution, and interactive visualization without managing any infrastructure.

## 🧩 Architecture Overview

The serverless data pipeline includes:
- **Amazon S3** for raw and processed data storage
- **AWS Glue Crawlers** for metadata extraction and cataloging
- **AWS Glue Jobs** for ETL processing (transforming raw data into queryable format)
- **Amazon Athena** for querying data using SQL and creating logical views
- **Amazon QuickSight** for data visualization and dashboarding

## 📁 Project Structure

![AWSDataLake](https://github.com/user-attachments/assets/8727696b-8c7b-4bff-aed4-7b25f95bdd82)



## 🚀 Getting Started

1. **Upload Data to S3**  
   Upload your raw CSV or JSON data to an Amazon S3 bucket.

2. **Set Up AWS Glue Crawler For Raw Data**  
   - Configure a crawler to scan the S3 location of raw data
   - Create a database and run the crawler to generate the schema

3. **Create Glue ETL Job**  
   - Develop a Glue job to transform raw data into a queryable format (e.g., Parquet)
   - Store the processed data in a different S3 prefix
  
4. **Set Up AWS Glue Crawler For Transformed Data**  
   - Configure a crawler to scan the S3 location of raw data
   - Create a database and run the crawler to generate the schema

5. **Query with Athena**  
   - Use Athena to run SQL queries on the transformed data
   - Create views for aggregation or filtering

6. **Visualize with QuickSight**  
   - Connect QuickSight to Athena
   - Build visual dashboards using the views created

## ✅ Key Features

- Serverless architecture
- Automated schema detection with AWS Glue Crawlers
- SQL-based querying with Athena
- Business intelligence and reporting with QuickSight

## 🛠️ Tools & Services Used

- Amazon S3
- AWS Glue (Crawlers & Jobs)
- Amazon Athena
- Amazon QuickSight
- AWS IAM (for permissions)


