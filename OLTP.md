# OLTP database requirements and design


## OLTP database
OLTP database is generally used to handle every day business transactions of an organization like a bank or a super market chain. OLTP databases can be write heavy or may have a balanced read/write load.

## OLTP database requirements:
An OLTP database is expected to handle a huge number of transactions per second. Each transaction usually involves accessing (read/write) a small portion of the database, in other words the payload per transaction is small.

The time taken to execute a transaction usually called latency needs to be very less.

## OLTP database design:
The schema of an OLTP database is higly normalized so as to achieve a very low latency. To further improve the latency an OLTP database stores only the recent data like the last few week's data. They are usually run on storage that is very fast like SSD.

# Scenario
You are a data engineer at an e-commerce company. Your company needs you to design a data platform that uses MySQL as an OLTP database. You will be using MySQL to store the OLTP data.

## Objectives
In this assignment you will:

- design the schema for OLTP database.
- load data into OLTP database.
- automate admin tasks.

## Tools / Software
- MySQL 8.0.22
- phpMyAdmin 5.0.4

# Exercise - Design the OLTP Database
## Task 1 - Create a database.
Create a database named sales.
```
>CREATE DATABASE sales;
>USE sales;
```

## Task 2 - Design a table named sales_data.
Design a table named sales_data based on the sample data given.
![MySQL sample table](sampledata.png)


Create the sales_data table in sales database.

![MySQL create sales_data table](createtable.png)
