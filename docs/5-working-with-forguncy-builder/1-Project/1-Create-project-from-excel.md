---
layout: default
title: Create Project from Excel
parent: Project
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Project/Create-project-from-excel/
nav_order: 1
---

# {{ page.title }}

Forguncy allows you to load an Excel sheet into a new project. It automatically recognizes cells in excel and generates fields, list views, forms, etc that can be used as application screens. Also, the necessary tables are created automatically. Later, you can make changes as per the requirement.

![create-from-excel-new](/assets/images/product-images/project-create-from-excel-new.png)
{:.dropshadow}

- Go to **File** and click **New**.
- Select **From Excel sheet**.
- Choose the required Excel file and click **Open**
- Select sheets to import (if there are more than one sheet in an excel file) and click **OK**.

![project-create-from-excel](/assets/images/product-images/project-create-from-excel.gif)
{:.dropshadow}

- Remove the demo data from the sheet, if it contains any. This will improve the accuracy of the auto-detection of input fields in a later step. If there is no demo data, click **Next** to skip the step.
- Load excel data. In this step you can import some excel files that are filled by the previous excel template. This will import the data to the database. Press **Next**. This is not a mandatory step. You can skip if no data needs to be imported.
- Adjust Bindings. The data source is necessary for web applications. Forguncy will analyze the document, and give the suggested data table structure. Click the **Auto Detect** button, if it doesn't initiate the data binding step. 
    
Note: Editing the value of the cell can change the column name.
{:.note}

You can always add a binding column or detail table later on (manually). 

It is recommended to read [Database](https://docs.forguncy.net/working-with-database/) and [Listview](https://docs.forguncy.net/working-with-forguncy-builder/List-views) features before for better understanding of this step.

- If Forguncy does not find any binding filed, you can not finish this step. Click on **Add Filed** to add and move to the next step.
- The next step is to adjust cell types. By default, Forguncy will generate editor cell type for binding fields i.e., the cell type is **Textbox** and the generated column data type will be text. You can change the cell type to **Number**, **Date**, or **Time**. In such a case, the column data type will be Number Type or Date type.    
- Click **Next** and move to table and page settings. Here, you can specify details for the table, select related pages, and merge Add/edit page. 

Note: The sheet name should be within 30 characters to generate pages.
{:.note}

- Click **Finish** to save entries and finish settings.

Note: *List* and *Registration* pages are created by default. *Details* and *Edit* pages can be selected.
{:.note}

Forguncy will create a project and you can make changes as per the requirement. The well-organized your excel sheet is, the more efficient will be the project creation process. 




