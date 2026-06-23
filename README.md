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
