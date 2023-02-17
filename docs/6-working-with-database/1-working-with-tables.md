---
layout: default
title: Working with Tables
parent: Working with Database
permalink: /working-with-database/working-with-tables/
nav_order: 1
---

# {{ page.title }}

## How to create a table

There are several ways to create a table. Follow below steps to create a new table:

### Create a New Table

- Go to **Create** tab and click **Table** dropdown.

![database_new_table](/assets/images/product-images/database_new_table.png)
{:.dropshadow}

- Choose the required option from the dropdown list. Select *New Table* to create a table in Forguncy's Internal Database. 
Select *New Linked Table* to create a new table in the external database. For connection settings to an external database, choose *Create External Table copy..*. 
- Configure the connection settings for the target external database of the copy table to be created.
- Clicking on *Create External Table copy..* or *New Linked Table* will open a dialog box. 
- Select required data source from the options listed on the dialog box. 

![database_new_table-data-source](/assets/images/product-images/database_new_table-data-source.png)
{:.dropshadow}

If you create a MySQL table, the table's storage engine will be "InnoDB".

The following fields are added automatically, when you create a table:
- **SQL Server, MySQL**: *FGC_Creator, FGC_CreateDate, FGC_LastModifier, FGC_LastModifyDate, FGC_UpdateHelp, FGC_Rowversion*
- **Oracle Database, PostgreSQL**: *FGC_Creator, FGC_CreateDate, FGC_LastModifier, FGC_LastModifyDate, FGC_UpdateHelp*

When creating an Oracle Database table, the *ID* field is not auto-incremented on creating a new record. You need to use Forguncy's automatic numbering function to set a unique value, or create a trigger for automatic numbering on the Oracle Database side with reference to the following code.

CREATE SEQUENCE table1_seq START WITH 1; <br/> CREATE OR REPLACE TRIGGER table1_id_trigger <br/> BEFORE INSERT ON table1 <br/> FOR EACH ROW <br/> BEGIN <br/> SELECT table1_seq.NEXTVAL <br/> INTO : new.id <br/> FROM dual; <br/> END;     
{:.note}

Alternatively, right-click the **Tables** tab in the navigation Pane and select **New Table** to create one in the Forguncy's internal database.

- Forguncy automatically assigns a sequential number to the table name (eg "Table 1"). You can rename a table by right-clicking the table name and selecting Rename.

![database_new_table-rename](/assets/images/product-images/database_new_table-rename.png)
{:.dropshadow}

Note: As in Excel, you can also rename by double-clicking the tab at the bottom of the workspace.
{:.note}


### Create Table from Excel File 


