
# Spark ETL Workflow
This project showcases an extract, transform, and load (ETL) data using PySpark and SparkSQL by adopting a star schema design (with a slight snowflake design on the product side).

### Project Description
This project presents an end-to-end ETL workflow on Databricks using PySpark and SparkSQL, illustrating how to extract, transform, and load (ETL) data.

### 1. Data Extraction:
- The source data is stored in CSV format on the Databricks Distributed File System (DBFS).
- The pipeline ingests six CSV files into a Spark environment for further processing.

### 2. Data Transformation:
- PySpark’s distributed processing power is used to perform data blending, filtering, aggregation, and apply business logic.
- Data is filtered to include only “Accessories” categories and “United States” country records.
- Rolling up the data to the customer level to show aggregated total sales and total quantity metrics per customer across the filtered dataset.
- The star schema design employs one fact table (storing the core transactional data) and five dimension tables with a slight snowflake schema on the product dimension.

### 3. Data Loading:
- The transformed data is then loaded into output folder of dbfs' FileStore.

Conclusion, By combining PySpark/SparkSQL, and a well-defined star schema with a slight snowflake extension for the product dimension, the project demonstrates an efficient end-to-end ETL workflow on Databricks.

## Data Model
Fact Table:
- [Sales.CSV](https://github.com/Lohithgk/Data_Engineering/blob/main/Datasets/Sales.csv)

Dimension Tables:
- [Products.CSV](https://github.com/Lohithgk/Data_Engineering/blob/main/Datasets/Products.csv)
- [Product_Subcategories.CSV](https://github.com/Lohithgk/Data_Engineering/blob/main/Datasets/Product_Subcategories.csv)
- [Product_Categories.CSV](https://github.com/Lohithgk/Data_Engineering/blob/main/Datasets/Product_Categories.csv)
- [Territories.CSV](https://github.com/Lohithgk/Data_Engineering/blob/main/Datasets/Territories.csv)
- [Customers.CSV](https://github.com/Lohithgk/Data_Engineering/blob/main/Datasets/Customers.csv)

  ![Data Model](https://github.com/Lohithgk/Data_Engineering/blob/main/Docs/Data%20Model.jpg)

## Script
- [Workflow using PySpark](https://github.com/Lohithgk/Data_Engineering/blob/main/Scripts/Workflow%20using%20PySpark.ipynb)
- [Workflow using SparkSQL](https://github.com/Lohithgk/Data_Engineering/blob/main/Scripts/Workflow%20using%20SparkSQL.ipynb)

## Script Weblink
- [Workflow using PySpark](https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/3690907634854246/2866696411247148/8959865570045467/latest.html)

- [Workflow using SparkSQL](https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/3690907634854246/3201828467364194/8959865570045467/latest.html)
