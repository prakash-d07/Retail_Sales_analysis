# Retail_Sales_analysis

"The Retail Data Analysis Dashboard."  This comprehensive, automated retail analysis model allows clients to upload data in AWS server and receive real-time updates in Power BI. This automated process helps to  Gain valuable insights into customer buying patterns and seasonal trends effortlessly.

This fully functional automated Retail Analysis Model involves 6 major steps:

1. Setting up Amazon Web Services (AWS):
-- The client tries to set up AWS and then seamlessly uploads all raw files into the bucket.
-- Implemented appropriate roles and policies, enabling secure access to the bucket and performing essential operations such as creating user-specific folders and uploading data. 

2. Step in Snowflake (SQL):
-- Conducted table creation and established storage integration and staging procedures to establish a connection with AWS.
-- Connected AWS S3 to Snowflake by creating a storage integration and pipe, facilitating continuous data upload tracking by automatically creating corresponding tables in Snowflake.
-- Set up a snow pipe to recognize and ingest files from the external stage, copying the data into the existing table. ❄️

3. Step in Jupyter_Notebook (Python):
--Established a seamless connection between Snowflake and Jupyter Notebook to retrieve data from tables into separate DataFrames.
-- Conducted Exploratory Data Analysis (#EDA), which involved data cleaning, modification, and in-depth analysis.
-- Stored the cleaned data back into Snowflake using the snowflake-python package within the same existing schema from which the data was extracted from the S3 bucket. 📊🐍

4. Step in #Jupyter_Lab (#Python):
--Utilized the jupyter_scheduler and jupyterlab-scheduler to automate the EDA process and avoid repetitive commands, enabling scheduled refreshes in Jupyter Lab. ⏰🔄

5. Step in Snowflake (#SQL):
--Created a master Fact table and implemented several Key Performance Indicators (KPIs) in Snowflake using the cleaned data. 📈🔑

 6th Step in #PowerBI:
-Seamlessly connected the clean data, master table, and KPIs from Snowflake to Power BI.
- Leveraged the power of #DAX (Data Analysis Expressions), measures, new columns, parameters, and more within Power BI to create an intuitive and insightful dashboard 📊💡💻
- 
