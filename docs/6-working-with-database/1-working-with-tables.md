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

- [Create a New Table](#create-a-new-table)
- [Create Table from Excel File](#create-table-from-excel-file)
- [Create Table from Text File](#)

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
- Specifying multiple files- *picture1.jpg|picture2.jpg*
- Specifying multiple folders- *folder1|folder2*

### Create Table from Text File 

- Prepare a text file. You can import tab-delimited files as well as comma-delimited files.
- Click the **Text File to Table** button on the **Data** ribbon tab.
- Click the **Browse...** button to specify the file to import, confirm that [Import source data into a new table in the current database] is selected, and click the **OK** button.