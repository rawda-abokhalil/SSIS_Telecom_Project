# SSIS_Telecom_Project
Overview

This project is an ETL pipeline built with SQL Server Integration Services (SSIS) to process raw telecom transaction data (IMSI, IMEI, LAC, CELL, Event Type, Event Timestamp, etc.). It focuses on data cleaning, transformation, and loading into SQL Server for analytics and reporting.

Features

Extracts raw data from Flat File Sources (CSV/TXT).

Cleans records by replacing blanks and invalid values with NULL.

Converts data types (string → integer, string → date) for consistency.

Handles special cases such as lac == 0 or event_type == "".

Loads standardized data into SQL Server tables.

Use Case

Telecom operators generate huge volumes of logs daily. This project ensures that raw data is transformed into a clean, reliable dataset ready for business intelligence, reporting, and machine learning use cases.

Technologies

SQL Server Integration Services (SSIS)

SQL Server Database

Flat File Sources (CSV/TXT)

Workflow

Extract telecom data from flat files.

Transform using Derived Columns (replace blanks with NULL, cast values).

Load into SQL Server for downstream analytics.

Future Enhancements

Add error handling and logging.

Automate daily ingestion.

Build dashboards with Power BI.

📝 This project demonstrates practical ETL development in SSIS with a focus on telecom data quality and transformation.
