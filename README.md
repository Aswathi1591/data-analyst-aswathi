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

**6. Monitoring and Audit**
I explored CloudWatch to monitor resource usage and saw how CloudTrail captures API activity for auditing. This was useful in tracking events and understanding usage patterns in the system.

Overall, this project gave me hands-on experience in setting up a cloud-based descriptive analysis workflow. I not only learned how to use AWS tools effectively but also understood the importance of secure, automated, and scalable data handling in real-world scenarios.

**Insights and findings:**
Through the descriptive analysis of the Public Washroom dataset using AWS services, I was able to derive the following key insights:

Most public washrooms are concentrated in urban areas, with significantly fewer facilities in suburban or less populated regions.
A large number of entries lacked accessibility features, indicating potential gaps in inclusive infrastructure.
The facility types varied, with some being permanent, others portable or seasonal, a pattern that reflects different usage and maintenance requirements.
AWS Glue DataBrew helped me uncover several formatting inconsistencies and missing values, which I successfully resolved using transformation recipes.
Using Athena, I found that the majority of washrooms fall under a few dominant categories, and some facilities were repeated across multiple records, likely due to naming or address variations.

These findings provided me with a better understanding of how structured datasets can reveal practical patterns in public infrastructure planning and service availability.

**Recommendations:**
Based on my analysis and learnings, I would suggest the following improvements and future steps:

**Improve Data Standardization**
Use data validation rules or manual review to eliminate inconsistent naming and duplicate records, which can distort analysis.

**Enhance Accessibility Reporting**
Ensure every facility entry includes accessibility metadata, as this is critical for inclusive public service planning.

**Increase Coverage in Underserved Areas**
Consider expanding facility availability in suburban or rural zones to improve service equity and public hygiene access.

**Use Parquet Format for Analytics**
For future analytics, I recommend storing data in Parquet + Snappy, which provides better compression and performance for large datasets.

**Automate Monitoring and Alerts**
Set up SNS notifications with CloudWatch and CloudTrail for real-time visibility into job failures, unusual access patterns, or security events.

**Tool & Technologies**
For this project, I primarily used Amazon S3 to store both raw and processed data securely in the cloud. AWS Glue DataBrew was instrumental in cleaning and transforming the dataset through visual recipe jobs, while the AWS Glue Data Catalog helped organize metadata for easy access. I performed SQL queries on the transformed data using AWS Athena, which enabled efficient, serverless analysis directly from S3. To ensure data security, I used AWS Key Management Service (KMS) for encryption and S3 versioning to maintain data integrity. Monitoring was handled through Amazon CloudWatch, and user activity was logged using AWS CloudTrail. The final outputs were stored in both Parquet (Snappy) and CSV formats to balance performance with readability. Tools like Draw.io were also used to visualize the AWS architecture and data pipeline structure.

**Conclusion**
This project provided me with a hands-on opportunity to apply descriptive analysis techniques to a real-world dataset using cloud-native tools. By working with AWS services such as S3, Glue DataBrew, and Athena, I gained a deeper understanding of how cloud platforms can streamline data storage, transformation, and analysis processes. I was able to identify meaningful patterns in the public washroom dataset, including facility distribution, accessibility gaps, and metadata inconsistencies. Beyond the analytical insights, this project also strengthened my skills in data governance, security, and infrastructure monitoring through tools like AWS KMS, CloudTrail, and CloudWatch. Overall, this experience has not only enhanced my technical capabilities in cloud computing and data analysis but also highlighted the importance of secure, scalable, and well-structured data pipelines in driving data-driven decision-making.






