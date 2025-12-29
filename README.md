# DE_AWS_CarePlusDataStores

# Data Engineering Pipeline for Analytics Consumption

## Objective
The objective of this project is to understand **how data reaches a Data Analyst** by implementing the **data engineering steps prior to analytics**.  
The focus is on ingestion, processing, storage formats, access control, and delivery of analytics-ready data.

---

## Project Overview
Raw support log data was ingested into cloud storage, processed using AWS services, stored in an optimized columnar format (Parquet), and prepared for downstream analytical consumption.

This project demonstrates how data engineering decisions directly impact usability for data analysts.

---

## Data Flow Summary
- Raw log files ingested into **Amazon S3** using a batch-based approach
- Data processed using **AWS Lambda**
- Processed data stored in **Parquet** format
- Parquet outputs converted to **CSV** for BI tool compatibility
- Parquet to CSV Conversion Tool:
https://www.agentsfordata.com/parquet/to/csv


---

## AWS Services & Security
- **Amazon S3** used as the raw and processed data lake
- **AWS Lambda** handled lightweight ETL processing
- **AWS Glue Data Catalog** used for schema understanding
- **AWS IAM** roles and policies managed secure service-to-service access following least-privilege principles

---

## Challenges & Constraints
- Unable to proceed with **Amazon Redshift** due to AWS free-tier subscription limitations
- Faced service configuration and permission constraints while integrating advanced query layers
- These limitations influenced the decision to focus on S3-based delivery and format materialization

---

## Scope Clarification
This project focuses strictly on **data engineering workflows** — ingestion, processing, storage, and delivery.  
Business analytics, dashboards, and KPI modeling are intentionally kept out of scope.

---

## Project Status
✅ Data ingestion completed  
✅ Processing and Parquet generation completed  
✅ Analyst-ready data delivery achieved  

**Project completed for defined scope.**

---

## Tech Stack
- Amazon S3  
- AWS Lambda  
- AWS Glue
- AWS IAM  
- Parquet  
- CSV  

---

AWS S3 Buckets:
https://ap-south-1.console.aws.amazon.com/s3/home?region=ap-south-1

AWS Glue:
https://eu-north-1.console.aws.amazon.com/gluestudio/home?region=eu-north-1#/editor/job/ETL_Support_Tickets/graph

AWS Lambda:
https://eu-north-1.console.aws.amazon.com/lambda/home?region=eu-north-1#/functions/support_log_ETL?tab=code

AWS IAM:
https://us-east-1.console.aws.amazon.com/iam/home?region=ap-south-1#/roles


