---
layout: default
title: Create from Excel
parent: Project
grand_parent: Develop
permalink: /develop/Project/Create-from-excel/
nav_order: 1
---

# {{ page.title }}

Load an Excel sheet into a new project, automatically recognize cells in Excel, automatically generate fields and list views that will be used as application screens, automatically generate each page (registration, list, details, edit), and necessary tables will be automatically created.

You can make changes to create your own applications.

![create-from-excel-new](/assets/images/product-images/project-create-from-excel-new.png)
{:.dropshadow}

- Go to **File** and click **New**.
- Select **From Excel sheet**.

![import-excel-select-page](/assets/images/product-images/import-excel-select-page.png)
{:.dropshadow}

- Choose the required Excel file and click **Open**
- Select sheets to import and click **OK**.

![project-create-from-excel](/assets/images/product-images/project-create-from-excel.gif)
{:.dropshadow}

- Remove the demo data from the sheet, if it contains any. This will improve the accuracy of the auto-detection of input fields in a later step. If there is no demo data, click **Next** to skip this step.
- Load excel data. You can import some excel files that are filled by the template. After import, the data will be imported to the database. Press **Next** to skip this step if no excel file needs to import or to proceed.
- Adjust Bindings. The data source is necessary for web applications. Click the **Auto Detect** button. Forguncy will analyze the document, and give the suggested data table structure. You can add a binding column or detail table manually.
    
Note: Editing the value of the cell can change the column name.
{:.note}

- If Forguncy does not find any binding filed, you can not finish this step. Click on **Add Filed** to add and move to the next step.
- The next step is to adjust cell types. By default, Forguncy will generate editor cell type for binding fields i.e., the cell type is **Textbox** and the generated column data type will be text. You can change the cell type to **Number**, **Date**, or **Time**. In such a case, the column data type will be Number Type or Date type.    
- Click **Next** and move to table and page settings. Here, you can specify details for the table, select related pages, and merge Add/edit page. 
- Click **Finish** to save entries and finish settings.

Note: *List* and *Registration* pages are created by default. *Details* and *Edit* pages can be selected.
{:.note}






