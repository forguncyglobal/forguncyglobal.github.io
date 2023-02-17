---
layout: default
title: Working with Database
permalink: /working-with-database/
nav_order: 6
has_children: true
has_toc: true
---

# {{ page.title }}

## Basic Knowledge of Database

A database collects, saves, and manages data for a specific purpose so that it can be easily accessed by executing search or extract commands. Database makes data retrival easy and flexible for the business. 

![tables-tab](/assets/images/product-images/tables-tab.png)
{:.dropshadow}

The key elements of a database are as follows:

|**Table**|A table is a collection of data that stores various data types in a database in tabular format. The table has an appearance and structure similar to Excel, so anyone can easily handle the database. You can save the data you enter on the page to a table, and you can display and edit the data saved in the table on the page. The concept is almost similar to an Excel table, with vertical columns called fields and horizontal rows called records.<br/> A table can have multiple fields and can store multiple records.|
|**Field**|A field is an item for storing different types of data separately. Fields are typically data-typed.<br/> Forguncy has nine types: Text, Integer, Decimal, Date/Time, Time, Yes/No, User Account, Image, and Attachment.|
|**Record**|A record is a unit of a collection of data for one record. If there are 3 records in the customer table, it means that the data for 3 customers is stored.|
|**Primary key**|A unique field that identifies a record in a table.|
|**Foreign key**|A field used for association with other tables. A foreign key must be a primary key in the table to which it is related.|

## Forguncy Database

Forguncy has an internal database, there is no need to prepare a new database, and applications can be developed using only Forguncy database. Although, you can connect to an external databases via SQL Server, Oracle Database, MySQL, PostgreSQL, or ODBC data sources if required. 
