# 🍏 **Apple Sales Data Engineering Project**

---

## 📌 **Project Overview**

Welcome to the **Apple Sales Data Engineering Project** — an end-to-end ETL pipeline created to extract meaningful business insights from simulated Apple sales data. While the dataset is **imaginary**, it is crafted to reflect real-world business scenarios and customer behaviors, making it ideal for **learning and prototyping**.

---

## 🏗️ **ETL Pipeline Architecture**

This project implements a classic **ETL (Extract, Transform, Load)** architecture using:

- **Databricks**
- **Apache Spark**
- **PySpark**

---

## 📁 **Dataset Overview**

Three core datasets drive the analytic insights:

- **Customer.csv** – Customer ID, name, gender, age, and region
- **Products.csv** – Product ID, name, category (e.g., iPhone, MacBook), and price
- **Transactions.csv** – Records each sale, linking customer & product with date, quantity, and revenue

Together, these datasets enable analysis of:

- Customer purchasing behavior
- Product performance
- Overall sales trends

---

## 🔧 **ETL Pipeline Breakdown**

### 1️⃣ **Extraction**

- **Platform:** Databricks File System (DBFS)
- **File Formats Used:** Delta, Parquet, CSV
- **Extractor_Notebook:** Handles all data ingestion from DBFS
- **Reader_Factory:** Dynamically detects and ingests files in the required format at runtime for maximum modularity and control

### 2️⃣ **Transformation**

- **Technology:** PySpark on Databricks (Apache Spark)
- **Transformation_Notebook:** Contains all business logic and DataFrame/SparkSQL transformations
- **Key Analytics Pipelines:**
    - Customers who purchased **AirPods after buying an iPhone**
    - Customers who purchased **both AirPods and iPhone**
    - List of **all products bought by a customer after their initial purchase**
    - **Average time delay** between buying an iPhone and then AirPods (per customer)
    - **Top 3 selling products** in each category by total revenue

### 3️⃣ **Loading**

- **Platform:** DBFS
- **Loader_Factory:** Dynamically identifies file format for saving
- **Loader_Notebook:** Writes final output data back to DBFS using **Delta Lake** and **Data Lake** formats for durability & scalability

---

## 🚧 **Notes & Future Enhancements**

- This project utilizes **fictional Apple sales data** strictly for educational purposes and Spark learning.
- **Planned extensions** include:
    - Workflow orchestration & scheduling
    - Automated data validation
    - Deeper business intelligence features

---

## 🤝 **Contributions & Feedback**

Ideas, suggestions, or feedback? **Feel free to raise an issue or connect for collaboration!**

---

## 📌 **Disclaimer**

All data is **synthetic** and intended **solely for learning and prototyping**. Not for commercial or production use.

---
