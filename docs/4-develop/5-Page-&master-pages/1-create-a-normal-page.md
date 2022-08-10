---
layout: default
title: Create A Normal Page
parent: Page &amp; Master Pages
grand_parent: Develop
permalink: /develop/Page-&-master-pages/create-a-normal-page/
nav_order: 1
---

# {{ page.title }}

- [Create A New Page](#create-a-new-page)
- [Create Page From Excel](#create-page-from-excel)
- [Create Page From Table](#create-page-from-table)

## Create A New Page

Steps to create a new web page are:
- Go to **Create** and select **Page**.
- A new page with defalut name (*Page 1, Page 2..*) will be added in the navigation bar. 
![create-new-page](/assets/images/product-images/create-normal-page.png)
{:.dropshadow}
- Right-click on the page name and select **Rename** to rename the page.
- Open pages are displayed in tabs below the workspace. You can switch pages by clicking the tabs.
![open-page-tab](/assets/images/product-images/open-page-tab.png)
{:.dropshadow}

Note: You can also rename by double-clicking the tab at the bottom of the workspace, just like in Excel.
{:.note}

## Create Page From Excel

You can import an Excel file into your page in two ways:

1. Drag and drop the Excel file you want to import onto the Forguncy page.
    ![import-excel-page](/assets/images/product-images/import-excel-page.png)
    {:.dropshadow}

    ![import-excel-select-page](/assets/images/product-images/import-excel-select-page.png)
    {:.dropshadow}
2. Import the Excel file from Forguny's Data tab:
    ![data-from-excel](/assets/images/product-images/data-from-excel.png)
    {:.dropshadow}
- Prepare an Excel file to import.
- Go to **Data** and click on **From Excel**.
- Browse the Excel file to import. You can also import multiple sheets.
- **Import Speardsheet Wizard** dialoge will appear.
    ![data-from-excel](/assets/images/product-images/import-spreadsheet-wizard.png)
    {:.dropshadow}
- Select the excel sheet or range that you want to import.
- You can also specify name of the import table.
- Click on **Finish** to create the page.

When reading password-protected Excel file, enter the correct password and click on **OK** to read the data.
{:.note}

Note: Forguncy supports only following items in Excel. Items that are not mentioned here will not be reflected on loading.
{:.note}

|line|height|
|column|width|
|cell|value formula vertical join horizontal join hyperlink Background color text color font font size Font style ([Normal] style only) Underline Strikethrough indentation character wrapping ruled line vertical alignment horizontal alignment data validation|
|sheet|image * If the Excel file to be imported is an XLS file (Excel 97 - 2003 workbook), the image will not be reflected. page settings|
{:.note}

## Create Page From Table

Based on the field configuration of the specified table, you can automatically generate the web pages to display data or update the table.
Using this function, you can create a four types of pages: 
1. List page
2. Detail page
3. Registration page
4. Edit page.
<!-- For tables with detail tables in master-detail relationships, detail list views are auto-generated on detail pages, registration pages, and edit pages. You can edit and drag items on the edit page and the details list view on the registration page. 

Note: If the table from which the page is generated has the following fields, by assigning the field types to different types , images and attachments can be displayed, or user account information can be separated into individual fields. You can 
{:.note}
- There is a string type field that holds the full path of the attached file and image file in the external database table
- An external database table has a String type field that holds user account information
{:.note} -->

Steps to create a web page from table are:

- Go to **Create** and select **Page From Table**.
    ![from-table-page](/assets/images/product-images/from-table-page.png)
    {:.dropshadow}
- Select table to generate page.
    ![from-table-page](/assets/images/product-images/from-table-created-page.png)
    {:.dropshadow}

<!-- Note: To generate the "Register" and "Edit" pages as one common page, check "Generate registration and update as one page".
{:.note} -->

The related following pages are automatically created. You can edit them as required.
- List page
- Details page
- Registration page
- Edit page

    ![from-table-page](/assets/images/product-images/from-table-created-page-2.png)
    {:.dropshadow}
