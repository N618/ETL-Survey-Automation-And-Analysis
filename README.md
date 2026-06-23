# Kerala Election Survey Analytics & ETL Automation

<p align="left">

<img src="https://img.shields.io/badge/PYTHON-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white"/>
<img src="https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apache-spark&logoColor=white"/>
<img src="https://img.shields.io/badge/POWER%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black"/>
<img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white"/>
<img src="https://img.shields.io/badge/GLUE-FF9900?style=for-the-badge"/>
<img src="https://img.shields.io/badge/ATHENA-4B8BBE?style=for-the-badge"/>
<img src="https://img.shields.io/badge/S3-569A31?style=for-the-badge&logo=amazon-s3&logoColor=white"/>
<img src="https://img.shields.io/badge/WEIGHTIPY-6A5ACD?style=for-the-badge"/>
<img src="https://img.shields.io/badge/JUPYTER-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>

</p>

---

## Overview

This project is a large-scale survey analytics and automation pipeline built for a Kerala election CAPI survey workflow.  
It combines **Survey CTO data extraction**, **ETL automation**, **AWS-based storage and querying**, **Power BI reporting**, and **advanced voter analysis on weighted survey data**.

The project was designed to solve a key operational problem: manually downloading survey data from Survey CTO was slow and time-consuming.  
By automating the entire flow, the process became faster, more reliable, and scalable for daily monitoring and analysis.

---

## Project Highlights

- Processed **10+ lakh survey records**
- Worked with **1+ crore electoral records**
- Automated **data extraction, cleaning, validation, and reporting**
- Reduced manual processing effort by **87%**
- Built vendor-level and agent-level performance tracking dashboards
- Performed advanced voter analysis on weighted data
- Enabled daily quota monitoring and sample validation checks

---

## Objective

- Automate Survey CTO data extraction
- Clean and standardize raw survey responses
- Upload structured data to AWS S3
- Use AWS Glue crawler to catalog the data
- Query the dataset through Athena
- Connect Athena tables to Power BI using ODBC
- Build interactive dashboards for operational monitoring
- Perform weighting and deep-dive voter analysis on valid samples
- Support election research through data-driven insights

---

## Data Sources

This project uses multiple survey and electoral sources, including:

- Survey CTO CAPI survey data
- Valid and invalid sample records
- Electoral reference data
- Past election result mappings
- Demographic and caste-related reference tables
- Alliance mapping files
- Weighted survey output datasets

---

## Project Structure

```text
Kerala-Election-Survey-Analytics
│
├── README.md
├── LICENSE
├── requirements.txt
├── .gitignore
│
├── notebooks
│   ├── Survey_API_Integration_Automation.ipynb
│   └── Weighing.ipynb
│
├── data
│   ├── raw
│   ├── processed
│   └── weighted
│
├── outputs
│   ├── dashboard.png
│   ├── sample_validation.png
│   ├── agent_tracker.png
│   ├── retention_analysis.png
│   └── deep_dive_analysis.png
│
├── reports
│   ├── Survey_ETL_Report.pdf
│   └── Weighted_Analysis_Report.pdf
│
├── sql
│   ├── athena_queries.sql
│   └── validation_queries.sql
│
└── powerbi
    └── survey_vendor_rls.pbix
End-to-End Workflow
Survey CTO
    ↓
API Extraction
    ↓
Automated Data Cleaning
    ↓
Validation & Transformation
    ↓
Upload to AWS S3
    ↓
AWS Glue Crawler
    ↓
Athena Tables
    ↓
ODBC Connection
    ↓
Power BI Dashboard
    ↓
Daily Vendor / Agent Monitoring




ETL Automation

The first part of the project focused on building an automated ETL pipeline.

What was automated
Survey CTO data extraction through API
Scheduled downloads
Data preprocessing and standardization
Uploading cleaned files to AWS S3
Glue crawler execution
Athena table refresh
Dashboard-ready data availability
Business impact

This automation removed repeated manual downloading and reduced processing time significantly, improving operational efficiency and reporting speed.

Power BI Dashboard

An interactive Power BI dashboard was created to track survey operations.

Dashboard features
Vendor-wise performance tracking
Daily quota monitoring
Valid / invalid sample detection
Agent-wise sample spread
Operational status overview
Survey completion monitoring

This helped the team track performance daily and identify issues early.

Data Preparation

The notebook includes preprocessing steps such as:

Checking missing values and duplicates
Removing invalid responses
Filtering non-audio invalid and audio invalid samples
Cleaning column names and values
Handling blank or inconsistent records
Standardizing text fields
Mapping party labels to alliances
Creating usable analysis-ready datasets
Weighted Analysis

The second part of the project focused on analysis of valid samples.

Steps performed
Exploratory Data Analysis on valid survey data
Normalization of demographic fields
Gender normalization
Age bucketing
Caste grouping
Past election result mapping
Survey weighting using weightipy
Alliance-wise and constituency-wise evaluation
Deep-dive analysis included
Retention analysis
A/B testing
Demographic voting patterns
Voter behavior analysis
Confidence interval estimation
Party-wise vote share understanding
Analytical Use Cases

This project supports a wide range of election analytics use cases:

Sample quality monitoring
Vendor performance evaluation
Survey completeness validation
Weighted voter opinion analysis
Demographic segmentation
Party and alliance trend analysis
Field-level data governance
Technologies Used
Python
SQL
PySpark
AWS S3
AWS Glue
AWS Athena
Survey CTO API
Power BI
ODBC
Pandas
NumPy
Weightipy
Jupyter Notebook
Key Results
Automated survey data pipeline from Survey CTO to AWS and Power BI
Reduced manual effort by 87%
Enabled faster daily reporting and sample monitoring
Scaled analytics across 10+ lakh survey records
Supported deep analysis on 1+ crore electoral records
Improved data reliability and operational visibility
How to Run the Project
git clone https://github.com/your-username/Kerala-Election-Survey-Analytics.git
cd Kerala-Election-Survey-Analytics
pip install -r requirements.txt
jupyter notebook

Open the notebooks in the notebooks/ folder and run them step by step.

Notebook Details
Notebook	Purpose
Survey_API_Integration_Automation.ipynb	API extraction, preprocessing, S3 upload, Glue/Athena workflow
Weighing.ipynb	Cleaning, normalization, weighting, and deep-dive voter analysis
Conclusion

This project demonstrates a complete large-scale election analytics workflow, from survey extraction to cloud-based ETL automation, dashboard reporting, and weighted voter analysis.
It reduced manual work, improved processing speed, and enabled structured decision-making for election operations.

Author

Nitish Jha
Data Analyst | Python | SQL | PySpark | Power BI | AWS
