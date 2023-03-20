---
layout: default
title: Linked Table
parent: External Database
grand_parent: Working with Database
permalink: /working-with-database/external-database/linked-table/
nav_order: 1
---

# {{ page.title }}

In Forguncy, a table that connects to an external database is called a linked table.

- For a linked table to work properly, the destination table must have at least one column with a primary key or a unique non-nullable column. For SQL Server, Oracle Database, MySQL, and PostgreSQL, primary keys are automatically detected, but if you are using an ODBC data source, manually set the Unique Record Identifier (Primary key), it is important.

- It is recommended to not use the same name as a built-in field such as *Last Modified Time* or *Assignee* in Forguncy's table in an alias using the AS clause in the CREATE statement of the view. If you do so, Forguncy functionality will not work for those fields.

## Connection to External Database

Steps to connect to SQL server/ Oracle Database/ MySQL/ PostgreSQL are:

- Go to **Data** tab and select **External Data Source**. 

![data_tab_external_data_source](/assets/images/product-images/data_tab_external_data_source.png)
{:.dropshadow}

- Establish connection with the required source. 
- Set the connection settings in the dialog.

![external-data-source-connection-properties](/assets/images/product-images/external-data-source-connection-properties.png)
{:.dropshadow}

- Click on **Change..** to change data source.

![change-data-source](/assets/images/product-images/change-data-source.png)
{:.dropshadow}

- Click **OK** button to save.

## Mapped Data Type

|SQL Server Data Type|Forguncy Data Types|
|:--|:--|
|bit|Yes/No|
|decimal|Decimal|
|int|integer|
|tinyint|text|
|smallint|integer|
|bigint|integer|
|money|Decimal|
|small money|Decimal|
|numeric|Decimal|
|real|Decimal|
|float|Decimal|
|time|Times of Day|
|date|Date Time|
|datetime|Date Time|
|datetime2|Date Time|
|small date time|Date Time|
|datetimeoffset|text|
|char|text|
|nchar|text|
|nvarchar|text|
|nvarchar(max)|text|
|varchar|text|
|varchar(max)|text|
|text|text|
|ntext|text|
|Image|text|
|unique identifier|text|
|sql_variant|text|
|sysname|text|

|Datatypes in Oracle Database|Forguncy Data Types|
|:--|:--|
|CHAR|text|
|CLOBs|text|
|DATE|Date Time|
|INTERVAL DAY TO SECOND|Times of Day|
|NCHAR|text|
|NVARCHAR2|text|
|NCLOB|text|
|NUMBER(x, 0)|integer|
|NUMBER(x, y) *If y is greater than 0|Decimal|
|RAW|text|
|TIMESTAMP|Date Time|
|TIMESTAMP WITH LOCAL TIME ZONE|Date Time|
|TIMESTAMP WITH TIME ZONE|Date Time|
|VARCHAR|text|
|VARCHAR2|text|

|MySQL Data Type|Forguncy Data Types|
|:--|:--|
|BIGINT|integer|
|BIT|integer|
|CHAR|text|
|DATE|Date Time|
|DATETIME|Date Time|
|DECIMAL|Decimal|
|DOUBLE|Decimal|
|ENUM|text|
|FLOAT|Decimal|
|INTEGER (or INT)|integer|
|JSON|text|
|LONG TEXT|text|
|MEDIUMINT|integer|
|MEDIUM TEXT|text|
|REAL (or DOUBLE PRECISION)|Decimal|
|SET|text|
|SMALLINT|integer|
|TEXT|text|
|TIME|Times of Day|
|TIMESTAMP|For Concurrency Control in Forguncy, or Date/Time|
|TINYINT|integer|
|TINY TEXT|text|
|VARCHAR|text|
|YEAR|integer|

|PostgreSQL Data Types|Forguncy Data Types|
|:--|:--|
|BIT|Yes/No|
|BOOL|Yes/No|
|CHAR|text|
|DATE|Date Time|
|DECIMAL|Decimal|
|FLOAT4|Decimal|
|FLOAT8|Decimal|
|INT2|integer|
|INT4|integer|
|INT8|integer|
|INTERVAL|Times of Day|
|JSON|text|
|JSONB|text|
|JSONPATH|text|
|MONEY|Decimal|
|NUMERIC|Decimal|
|SERIAL2|integer|
|SERIAL4|integer|
|SERIAL8|integer|
|TEXT|text|
|TIME|Times of Day|
|TIMESTAMP|For Concurrency Control in Forguncy, or Date/Time|
|UUID|text|
|VARCHAR|text|
|XML|text|
|BPCHAR|text|
|REGCONFIG|integer|
|REGTYPE|integer|
|OIDs|integer|

