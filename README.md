
# Spark ETL Workflow

This project showcases an extract, transform, and load (ETL) data using PySpark and SparkSQL by adopting a star schema design (with a slight snowflake design on the product side).

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

Workflow using PySpark
(https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/3690907634854246/2866696411247148/8959865570045467/latest.html)

Workflow using SparkSQL
(https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/3690907634854246/3201828467364194/8959865570045467/latest.html)
