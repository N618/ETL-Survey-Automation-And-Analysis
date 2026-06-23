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

```
---
## End-to-End Workflow
```
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
```
---

## ETL Automation

The first part of the project focused on building an automated ETL pipeline.

### What was Automated

- Survey CTO data extraction through API
- Scheduled survey downloads
- Data preprocessing and standardization
- Uploading cleaned files to AWS S3
- AWS Glue crawler execution
- Athena table refresh
- Dashboard-ready data availability

### Business Impact

This automation removed repeated manual downloading and reduced processing time significantly, improving operational efficiency and reporting speed.

---

## Power BI Dashboard

An interactive Power BI dashboard was created to monitor daily survey operations.

### Dashboard Features

- Vendor-wise performance tracking
- Daily quota monitoring
- Valid / Invalid sample detection
- Agent-wise sample spread
- Operational status overview
- Survey completion monitoring

The dashboard enabled the operations team to monitor vendor performance in real time and quickly identify field-level issues.

---

## Data Preparation

The notebook includes the following preprocessing steps:

- Checking missing values and duplicates
- Removing invalid responses
- Filtering audio and non-audio invalid samples
- Cleaning column names and values
- Handling blank or inconsistent records
- Standardizing text fields
- Mapping party labels to alliances
- Creating analysis-ready datasets

---

## Weighted Analysis

The second phase of the project focused on analyzing valid survey responses using statistical weighting techniques.

### Steps Performed

- Exploratory Data Analysis (EDA)
- Demographic normalization
- Gender normalization
- Age bucketing
- Caste grouping
- Past election result mapping
- Survey weighting using **Weightipy**
- Alliance-wise and constituency-wise evaluation

### Deep-Dive Analysis Included

- Retention analysis
- A/B testing
- Demographic voter behavior
- Voter preference analysis
- Confidence Interval estimation
- Party-wise vote share estimation

---

## Analytical Use Cases

This project supports multiple election analytics use cases, including:

- Sample quality monitoring
- Vendor performance evaluation
- Survey completeness validation
- Weighted voter opinion analysis
- Demographic segmentation
- Party and alliance trend analysis
- Field-level data governance

---

## Technologies Used

- Python
- SQL
- PySpark
- AWS S3
- AWS Glue
- AWS Athena
- Survey CTO API
- Power BI
- ODBC
- Pandas
- NumPy
- Weightipy
- Jupyter Notebook

---

## Key Results

- Automated the Survey CTO to AWS ETL pipeline
- Reduced manual effort by **87%**
- Enabled faster daily reporting and sample monitoring
- Processed **10+ lakh survey records**
- Integrated **1+ crore electoral records**
- Improved operational visibility through Power BI dashboards
- Delivered weighted voter analytics for strategic decision-making

---

## How to Run the Project

```bash
git clone https://github.com/your-username/Kerala-Election-Survey-Analytics.git

cd Kerala-Election-Survey-Analytics

pip install -r requirements.txt

jupyter notebook
```

Open the notebooks inside the `notebooks/` directory and execute them sequentially.

---

## Notebook Details

| Notebook | Description |
|----------|-------------|
| **Survey_API_Integration_Automation.ipynb** | Survey CTO API integration, automated ETL pipeline, AWS S3 upload, Glue crawler, Athena integration, and Power BI data preparation |
| **Weighing.ipynb** | Data cleaning, demographic normalization, survey weighting using Weightipy, statistical analysis, and voter behavior insights |

---

## Conclusion

This project demonstrates a complete large-scale election analytics pipeline, covering Survey CTO data extraction, cloud-based ETL automation, Power BI reporting, statistical weighting, and advanced voter behavior analysis.

The solution significantly reduced manual effort, improved processing speed, and enabled data-driven decision-making for election strategy and field operations.

---

## Author

**Nitish Jha**

**Senior Data Analyst**

Python • SQL • PySpark • AWS • Power BI • Machine Learning
    ↓
Daily Vendor / Agent Monitoring
