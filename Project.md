# Data Engineering Capstone project on Coursera
The text provided here was copied from material from the course
---
---

# Introduction

The data platform architecture of an ecommerce company named SoftCart.
SoftCart uses a hybrid architecture, with some of its databases on premises and some on cloud.

## Process:

SoftCart's online presence is primarily through its website, which customers access using a variety of devices like laptops, mobiles and tablets.

-   All the catalog data of the products is stored in the MongoDB NoSQL server.

-   All the transactional data like inventory and sales are stored in the MySQL database server.

SoftCart's webserver is driven entirely by these two databases.

-   Data is periodically extracted from these two databases and put into the staging data warehouse running on PostgreSQL.

-   The production data warehouse is on the cloud instance of IBM DB2 server.

-   BI teams connect to the IBM DB2 for operational dashboard creation.

-   IBM Cognos Analytics is used to create dashboards.

-   SoftCart uses Hadoop cluster as its big data platform where all the data is collected for analytics purposes.

-   Apache Spark is used to analyse the data on the Hadoop cluster.

## Tools and Technologies:
Please click on the links below to see each section

-   [OLTP database - MySQL](OLTP.md)

-   [NoSql database - MongoDB](NoSQL.md)

-   [Staging Data warehouse – PostgreSQL](datawarehouse.md)

-   [Production Data warehouse – PostgresSQL or IBM DB2 on cloud](Production.md)

-   [Data Pipelines - Python ETL](ETL.md)

-   [Data Pipelines - Apache Airflow](Airflow.md)

-   [Business Intelligence Dashboard - IBM Cognos Analytics](Cognos.md)

-   [Big data analytics platform – Spark](Spark.md)



|  PREV : [README](README.md)  | NEXT : [OLTP database - MySQL](OLTP.md)
|---|---|
