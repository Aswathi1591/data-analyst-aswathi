# data-analyst-aswathi
**DESCRIPTIVE ANALYSIS**

**Project title:** Cloud-Based Descriptive Analysis of Public Washroom Infrastructure Using AWS Services

**Project description / Objective:** 
This project presents a comprehensive descriptive analysis of a public washroom dataset by leveraging scalable, secure, and cost-effective AWS services. The primary objective is to analyze certain features of public infrastructure using AWS Clous tools while demonstrating a structured data pipeline.

Using services such as Amazon S3, AWS Glue, DataBrew, and Athena, the project implements a complete ETL workflow—from data ingestion and transformation to storage and analysis. The dataset, once cleaned and processed, was queried using SQL via AWS Athena and visualized for insights regarding usage patterns, location distribution, and data quality.

Advanced cloud functionalities such as KMS-based encryption, lifecycle policies, versioning, and CloudWatch monitoring were configured to ensure data integrity, cost optimization, and auditability. The project highlights the practical integration of descriptive analytics with cloud data engineering to support infrastructure planning and operational decision-making.

**Dataset:**
The dataset used in this project is titled "Public Washrooms" and contains metadata on public restroom facilities, likely sourced from City of Vancouver open data portal. It includes structured information about washroom locations, accessibility, operational details, and facility types.

**Methodology**
In this project, I performed a descriptive analysis of the Public Washroom dataset using AWS services to understand its structure, key trends, and facility distribution. The following steps reflect my approach and learning throughout the process:

**1. Data Upload and Organization**
I started by uploading the dataset to an Amazon S3 bucket. I learned how to structure the storage using folders, manage object permissions, and apply lifecycle rules to move infrequently accessed data to lower-cost storage like Glacier.

**2. Data Cleaning with AWS Glue DataBrew**
Using AWS Glue DataBrew, I created and executed recipe jobs to clean and transform the dataset:
Removed duplicates and missing values
Standardized formats (e.g., facility names, accessibility indicators)
Gained a better understanding of how transformation steps are applied and tracked in the AWS environment.

**3. Storing and Managing Outputs**
I stored the cleaned outputs in Amazon S3 in both Parquet (Snappy) and CSV formats. I learned that Parquet is more storage-efficient for analytics, while CSV is easier for manual review and reports.

**4. Querying with AWS Athena**
To explore the dataset further, I used AWS Athena:
Ran SQL queries to check how many facilities were accessible
Counted washrooms by region and facility type.
Gained real-time insights without moving data outside S3

**5. Security and Governance**
To protect the data,
Enabled server-side encryption with AWS KMS
Configured bucket versioning to retain previous versions
Enabled access logging to track who accessed which objects




