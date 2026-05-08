# yesbank-postgresql-analysis
Python + PostgreSQL project for analyzing Yes Bank financial data using Pandas and SQL queries.
Yes Bank Financial Modelling & Analysis
Overview
This project focuses on the financial modelling and analysis of Yes Bank using Python, PostgreSQL, SQL, and Pandas. The objective of this project is to analyze the company’s financial performance, study important financial metrics, and derive meaningful business insights from the balance sheet data.
Project Objectives
Connect Python with PostgreSQL database
Import and manage financial datasets
Perform financial ratio analysis
Analyze assets, liabilities, reserves, borrowings, and equity
Build a structured financial modelling workflow
Generate insights for decision-making
Technologies Used
Python
PostgreSQL
Pandas
SQL
Psycopg2
PyCharm
Financial Metrics Analyzed
Equity Capital
Reserves
Borrowings
Total Assets
Other Assets
Debt to Equity Ratio
Asset Utilization Ratio
Database Connectivity
The project uses psycopg2 to establish a connection between Python and PostgreSQL.
import psycopg2
import pandas as pd

conn = psycopg2.connect(
    host="localhost",
    port="5432",
    dbname="postgres",
    user="postgres",
    password="your_password"
)

df = pd.read_sql("SELECT * FROM public.final_yesbank;", conn)

print(df)

conn.close()
Key Learning Outcomes
Financial data analysis using Python
SQL query execution and database handling
Financial modelling concepts
Ratio analysis and performance evaluation
Data cleaning and processing using Pandas
Conclusion
This project helped in understanding how financial modelling can be performed using real-world banking data. It also improved practical knowledge of SQL, database connectivity, and financial analysis using Python.
Author
Priyanshu Kumar Rao
