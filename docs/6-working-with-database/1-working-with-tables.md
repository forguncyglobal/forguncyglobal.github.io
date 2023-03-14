---
layout: default
title: Working with Tables
parent: Working with Database
permalink: /working-with-database/working-with-tables/
nav_order: 1
---

# {{ page.title }}

## How to create a Table and Views

There are several ways to create a table. Follow below steps to create a new table and a view:

- [Create a New Table](#create-a-new-table)
- [Create Table from Excel File](#create-table-from-excel-file)
- [Create Table from Text File](#create-table-from-text-file)
- [Create a View](#how-to-create-a-view)

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

- Prepare an Excel file to import.

![table-from-excel-file](/assets/images/product-images/table-from-excel-file.png)
{:.dropshadow}

- Click the **Excel to Table** button from the **Data** ribbon tab.

![excel-to-table](/assets/images/product-images/excel-to-table.png)
{:.dropshadow}

- Click the **Browse...** button to specify the file to import data.

![excel-to table-get-external-data](/assets/images/product-images/excel-to%20table-get-external-data.png)
{:.dropshadow}

- Specify how and where you want to store the data in the current project and click the **OK** button.
- Select a sheet or range to import and click the **Next** button.

![excel-to-table-import-spreadsheet-wizard](/assets/images/product-images/excel-to table-import-spreadsheet-wizard.png)
{:.dropshadow}

- Select whether to use the data in the first row as field names, and click the **Next** button.

![excel-to%20table-import-spreadsheet-wizard-column-headings](/assets/images/product-images/excel-to%20table-import-spreadsheet-wizard-column-headings.png)
{:.dropshadow}

- Specify the column to be imported or not. Set the name, and data type of the fields to be imported. and then click the **Finish** button.

![excel-to%20table-import-spreadsheet-wizard-column-import](/assets/images/product-images/excel-to%20table-import-spreadsheet-wizard-column-import.png)
{:.dropshadow}

- Excel data is imported into the specified table.

**Rules for importing into image type fields**

Only one file can be stored in an image type field.

- Extension of the image file to be imported- .art, .bmp, .cmx, .cod, .dib, .gif, .ico, .ief, .jfif, .jpe, .jpeg, .jpg, .pbm, .pgm, .png, .pnm, .pnz , .ppm, .ras, .rf, .rgb, .tif, .tiff, .wbmp, .xbm, .xpm, .xwd
- File name specification- *picture1.jpg*
- Specifying a path including folders- *folder1\picture1.jpg*

**Rules for importing into attachment type fields**

An attachment type field can store multiple files.

- File name specification- *document1.docx*
- Specifying a path including folders- *folder1\document1.docx*
- Specifying a folder- All files present in the folder will be imported.
- Specifying multiple files- *picture1.jpg, picture2.jpg,..*
- Specifying multiple folders- *folder1, folder2,..*

### Create Table from Text File 

- Prepare a tab-delimited text file.

![tab-delimated-text-file](/assets/images/product-images/tab-delimated-text-file.png)
{:.dropshadow}

- Click the **Text File to Table** button on the **Data** ribbon tab.

![table-from-text-file](/assets/images/product-images/table-from-text-file.png)
{:.dropshadow}

- Click the **Browse...** button to specify the file to import. Choose **Import source data into a new table in the current database** option and click the **OK** button.

![get-external-data-text-file](/assets/images/product-images/get-external-data-text-file.png)
{:.dropshadow}

- Select the required option and click the **Next** button. 

![import-text-wizard](/assets/images/product-images/import-text-wizard.png)
{:.dropshadow}

- Clicking **Options...** displays the dialog shown below and allows you to set some options.

![text-to-table-import-options](/assets/images/product-images/text-to-table-import-options.png)
{:.dropshadow}

- Select whether to use the data in the first row as field names, and click the **Next** button.

![text-to-table-import-text-wizard](/assets/images/product-images/text-to-table-import-text-wizard.png)
{:.dropshadow}

- Specify the column to be imported or not. Set the name, and data type of the fields to be imported. and then click the **Next** button.

![text-to-table-import-text-wizard-2](/assets/images/product-images/text-to-table-import-text-wizard-2.png)
{:.dropshadow}

- Specify the table name of the import destination and click **Finish**.

![text-to-table-import-text-wizard-3](/assets/images/product-images/text-to-table-import-text-wizard-3.png)
{:.dropshadow}

- Text data is imported into the specified table.

## How to create a View

A view is a virtual table without the actual table itself. You can extract or combine some fields of a table or multiple tables to make them look like a single table. A view is defined by a query consisting of SQL statements.

Note: The below sections are all about creating views on Forguncy's internal database, not views on an external database such as SQL Server or Oracle Database.
{:.note}

Steps to create a View are:

- Go to **Create**, click **View** and select **New View..**. Alternatively, right-click the *Tables & Views* tab in the Navigation Pane and select **New View..**.

![create-view](/assets/images/product-images/create-view.png)
{:.dropshadow}

- Enter the **View Name** and SQL statement in the space provided.

![new-view](/assets/images/product-images/new-view.png)
{:.dropshadow}

Elements of Forguncy like table name and item name can be used in SQL statements.

|Item name|Item name that can be used in SQL|
|:--|:--|
|Identification|Identification|
|Author|FGC_Creator|
|Creation date|FG_CreateDate|
|Last updated by|FGC_LastModifier|
|Last Modified|FGC_LastModifyDate|
|Situation|FGC_State|
|Manager|FGC_AssignTo|
|Line version|It can not be used.|
|Update helper|It can not be used.|

Note: You can rename a view after creating it by right-clicking the view name and selecting **Rename** or by double-clicking the tab at the bottom of the workspace.
{:.note}

- Right-click the view name and select **Set Primary Keys..**.

![view-set-primary-keys](/assets/images/product-images/view-set-primary-keys.png)
{:.dropshadow}

- Select a primary key and click **OK**.

![views-select-unique-record-identifier](/assets/images/product-images/views-select-unique-record-identifier.png)
{:.dropshadow}

### Create a User Information View

You can create a user information view that displays all user information created in the user account management screen.

User information view values ​​are read-only. It cannot add, update, or delete records. The primary key of the user information view is created with *Username*. The primary key cannot be changed. Only one user information view can be created in one project. The user information view items cannot be deleted or changed.

- Go to **Create**, click **View** and select **User Info View..**. Alternatively, right-click the Tables tab in the Navigation Pane and click **User Info View..**.

![views-user-info-view](/assets/images/product-images/views-user-info-view.png)
{:.dropshadow}

- A user information view is created. Rename it as required.

![user-info-view](/assets/images/product-images/user-info-view.png)
{:.dropshadow}

Note: You can rename a user info view after creating it by right-clicking the user info view name and selecting **Rename** or by double-clicking the tab at the bottom of the workspace.
{:.note}

