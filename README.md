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
