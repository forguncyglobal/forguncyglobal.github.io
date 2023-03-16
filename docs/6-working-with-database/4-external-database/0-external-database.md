---
layout: default
title: External Database
parent: Working with Database
permalink: /working-with-database/external-database/
nav_order: 4
has_children: true
has_toc: true
---

# {{ page.title }}

In addition to internal databases, Forguncy can use external databases such as SQL Server, Oracle Database, MySQL, PostgreSQL, or ODBC data sources. Database Basics explains basic database concepts for those new to databases. 

External database can be used:

- To easily create a new application using data in an existing database.
- To change or expand the existing database structure.
- To reference and update common data in multiple Forguncy apps.
- To handle large amount of data (2TB or more).
- When heavy concurrent write operations are required. 

## Access Rights

Depending on the type of external database, you may or may not be able to grant per-role permissions on tables and fields. 

- SQL Server, Oracle Database, MySQL, PostgreSQL allows role-based access control and workflow access based on permissions. Forguncy automatically creates the tables and fields needed to manage it against these external databases.
- For ODBC data sources you cannot grant per-role privileges on tables or fields i.e. you can not set permissions on workflows or tables when using ODBC data sources.
