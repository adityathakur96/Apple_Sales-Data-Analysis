# Apple_Sales-Data-Analysis

In this Data Engineering project I have worked upon the Apple-Sales data so to acquire some useful information which will give information about the buisness of Apples.*

So in this project i have made the ETL pipelines in which -

**EXTRACTION** with the help of DBFS(Databricks File System  ) in which i have stored the files of apple-sales data in the format of Delta , Parquet and CSV.
For this to happen i have made the Extractor_Notebook in which iam extracting the data from the dbfs also with the help of reader_factory iam reading the format of file sp that only that foramt appear which
I need at particular time.

**TRANSFORMATION** with the help of Databricks which built upon Apache Spark , so I have used the Pyspark as i medium to write the code on databricks by which i have made so transformations using SparkSQL and also other concepts of spark. 
by which iam getting useful result on the sales data, like some of the pipelines are

1) Customer who have brought Airpods After buying the IPhone.
2) Customer who have brought both the Airpods and IPhone.
3) List of all the products brought by customer after their initial purchase.**
4) Determine the average time delay for buying an Iphone and buying Airpods for each customer.**
5) Identify the top 3 selling products inn each category by total revenue.**

For this I have created the Tranformation_Notebook in that all the transformation is done.


**LOADING** of the results is also done with the help of DBFS , for this i have made the Loader_Factory by which again format of file is identified and Loader_Notebook by which the all the resulted data is going to DBFS. 
The format of the loading files are Delta lake and Data Lake. 


**Note: **
*  *: This project only have imaginary data of the sales it's not real.

* **: I'll be making these pipelines in future and work on this project timely to learn more.


