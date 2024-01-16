# Empowering-E-commerce-Advanced-Analytics-Infrastructure


## Introduction
This README provides an overview of the data platform architecture for SoftCart, an e-commerce company. The architecture is a hybrid model, utilizing both on-premises and cloud-based databases.

## Tools and Technologies

### Databases
- **OLTP Database**: 
  - *MySQL* - Manages online transaction processing.
- **NoSQL Database**: 
  - *MongoDB* - Stores catalog data for products.
- **Production Data Warehouse**: 
  - *IBM DB2 on Cloud* - Serves as the primary operational data repository.
- **Staging Data Warehouse**: 
  - *PostgreSQL* - Used for initial data staging and processing.

### Data Processing and Analytics
- **Big Data Platform**: 
  - *Hadoop* - Supports large-scale data storage and processing.
- **Big Data Analytics**: 
  - *Apache Spark* - Employed for advanced data analytics on Hadoop.
- **Business Intelligence Dashboard**: 
  - *IBM Cognos Analytics* - Creates operational dashboards.
- **Data Pipelines**: 
  - *Apache Airflow* - Manages and automates data movement.

## Process Overview

### Web Platform and Data Storage
SoftCart's online platform is accessible through devices such as laptops, mobiles, and tablets. MongoDB and MySQL are integral to the webserver's functionality, handling product catalog and transactional data, respectively.

### Data Staging and Warehousing
Data extracted from MongoDB and MySQL is processed in PostgreSQL before being transferred to the IBM DB2 cloud-based data warehouse.

### Business Intelligence and Analytics
Operational dashboards are generated using IBM Cognos Analytics, linked to the cloud data warehouse. The Hadoop cluster and Apache Spark facilitate extensive data analysis.

### Data Movement and ETL
ETL pipelines, orchestrated via Apache Airflow, enable efficient data transfer between the OLTP, NoSQL databases, and data warehouses.

---

