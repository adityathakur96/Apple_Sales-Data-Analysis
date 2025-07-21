# Apple_Sales-Data-Analysis

📌 Project Overview
In this Data Engineering project, I worked on Apple Sales data to extract meaningful business insights that reflect customer purchasing behavior and product performance. Although the dataset is imaginary, it has been designed to simulate real-world business scenarios for learning purposes.

The project follows a classic ETL pipeline architecture—Extraction, Transformation, and Loading—implemented using Databricks, Apache Spark, and PySpark.

🔧 ETL Pipeline Breakdown

1️⃣ Extraction

-> Platform: Databricks File System (DBFS)

-> File Formats Used: Delta, Parquet, CSV

-> I developed an Extractor_Notebook that handles data ingestion from DBFS.

-> To dynamically manage file formats, I implemented a Reader_Factory, which detects and reads only the required format at runtime, enhancing modularity and control.

2️⃣ Transformation

-> Technology: PySpark (running on Databricks, powered by Apache Spark)

-> I used a combination of SparkSQL and DataFrame transformations to extract insights from the data.

-> All transformation logic resides in the Transformation_Notebook.

-> Key transformation pipelines include:

-> Customers who purchased AirPods after buying an iPhone

-> Customers who purchased both AirPods and iPhone

-> List of all products bought by a customer after their initial purchase

-> Average time delay between buying an iPhone and then AirPods for each customer

-> Top 3 selling products in each category by total revenue

3️⃣ Loading

-> Platform: DBFS

-> I implemented a Loader_Factory to dynamically identify file formats for saving.

-> All final output data is written back to DBFS using the Loader_Notebook in Delta Lake and Data Lake formats for durability and scalability.

🚧 Note

-> This project uses fictional Apple sales data for educational purposes only.

-> I plan to extend and refine these ETL pipelines in the future to include features like orchestration, scheduling, and data validation for deeper learning.




