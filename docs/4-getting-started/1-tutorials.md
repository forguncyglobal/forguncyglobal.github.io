---
layout: default
title: Tutorials
parent: Getting Started
permalink: /getting-started/tutorials/
nav_order: 1
---

# {{ page.title }}

The working environment of Forguncy is similar to Microsoft excel. The lessons are divided into Baisc and Advanced levels. 

Follow the below mentioned steps to build a web application using Forguncy.
### Basic Lessons
- [Getting Started](#getting-started)
- [Create Table & List View](#create-table-&-list-view)
- [Create New Record Screen](#create-new-record-screen)
- [Update & Delete Records](#update-&-delete-records)
- [Excel-like Formulas](#excel-like-formulas)
- [Export To Excel](#export-to-excel)
- [Query Data](#query-data)
- [Publish To Server](#publish-to-server) 

### Advanced Lessons
- [Create Master Details](#create-master-details)
- [Calculated Fields](#calculated-fields)
- [Aggregated Fields](#aggregated-fields)
- [Charts](#charts)

## Getting Started
Let's create a simple static webpage with text and images!

<iframe width="560" height="315" src="https://www.youtube.com/embed/9ly1--3x53A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Go to **Lessons** and open **Getting Started**. Either you can follow on screen instructions or the steps mentioned below:

1. Go to **New** and click on **Blank** to create a new project.
2. Select cell range and merge them by clicking on **Alignment**->**Merge Cells**.
3. Enter text in the merged cells and format it as per the requirement via **Font** and **Alignment** tabs.
4. Select a cell for the image placement and go to the **Insert** tab.
5. Select **Picture** and choose an image file.
6. Click on **Home**->**Start** to check the result in the web browser.

**Note**: From Lesson 2 to 7, you will learn to create a simple application for managing contacts using Forguncy.
## Create Table & List View
The lesson is about creating a table and a screen for listing the data.
<iframe width="560" height="315" src="https://www.youtube.com/embed/DPpoRK37qNg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Go to **Lessons** and open **Create Table & List View**. Either you can follow on screen instructions or the steps mentioned below:

1. Go to **New** and click on **Blank** to create a new project.
2. Right-click on **Tables and Views** (available in **Object Explorer** navigation pane), and select **New Table**.
3. A table with **Add Field** column will appear. 
4. Right-click on **Add Field**, select **Text**, and enter column name.
5. Similarly, you can add as many columns as you want of other data types such as Text, Integer, Decimal, Date and Time, etc.
6. Fill data in columns one-by-one.
7. Next step is to create a data Listing Page. For this double-click on **Page1** to open a page.
8. Select cell-range and click on **Insert Listview**.
9. Select table from **Select Table** popup window.
10. Click on **OK** to create a listview area.
11. To define columns, make a cell selection in the second row, and click on **Binding**.
12. In **Binding Field**, select column name from the dropdown list.
13. Repeat step 11 and 12 to define other columns of the table.
14. To format table cell, right-click and select **Format Cells**.
15. Click on **Home**->**Start** to check the result in the web browser.

## Create New Record Screen
The lesson is about creating a page layout to enter a new record in the List view. 
<iframe width="560" height="315" src="https://www.youtube.com/embed/BudneVkDsgc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Go to **Lessons** and open **Create New Record Screen**. Either you can follow on screen instructions or the steps mentioned below:

1. Right-click on the page and select **New Page**.
2. To rename the new page, right-click on the page and select **Rename**.  
3. Enter the name as required.
4. Select a cell and enter field name. The name can be same as a column name of the table or something related to.
5. Select cell range next to the name entered above.
6. Go to **Cell Type** and specify cell type. 
7. Now, bind data with selected cell range. Go to **Binding**. Set **Page Data Source** and **Binding Filed**.
8. Similarly create area for other inputs.
9. Place button to perform add action. Select cell range, select **Cell Type** as button, and give the button name as "Add".
10. Select button and go to **Cell Type** (right pane)->**Commands**.
11. Select **Update Data Table** and **Add** radio button in **Command Window**.
12. Click on **New Command** and select **Command** as **Navigate**.
13. Select target page in **Select Page** filed and click on **OK**.
13. Go to the target page i.e. listview page to reflect enteries.
14. Select cell and enter text as "Add" 
15. Go to **Cell Type** and select **Hyperlink**. Click on **Cell Type** (right pane)->**Commands**.
16. Click on **New Command** and select **Command** as **Navigate**. 
16. Select target page in **Select Page** filed and click on **OK**.
17. Click on **Home**->**Start** to check the result in the web browser.

## Update & Delete Records
The lesson is about editing and deleting a record.
<iframe width="560" height="315" src="https://www.youtube.com/embed/6pb7S3lYGeY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Go to **Lessons** and open **Update & Delete Records**. Either you can follow on screen instructions or the steps mentioned below:

1. The layout of edit page is similar to the add page. Hence, right-click on the add page and select **Duplicate**.
2. Right-click on the duplicate page and select **Rename**.
3. Input name and press enter.
4. Rename "Add" button as "Edit" button.
5. Select "Edit" button and go to **Cell Type** (right pane)->**Commands**.
6. Select **Edit** radio button in **Command Window** and click on **Ok**.
7. Double-click on the listview page to create hyperlink for the transition from list screen to edit screen.
8. Select a cell-range next to the last column and second row of the listview.
9. Select hyperlink or button cell type.
10. Input "Edit" in the cell-range and go to **Cell Type** (right pane)->**Commands**.
11. In **Command Window**, select "Navigate" in **Command** and "Edit Page" in **Select page** field.
12. To include delete functionality follow the same steps from 8 to 10. Input ""Delete" in place of "Edit".
13. Select **Delete Record** **Command** in the **Command Window** and click on **Ok**.
14. Click on **Home**->**Start** to check the result in the web browser.

## Excel-like Formulas
Learn how to set formula in Forguncy like excel. Forguncy supports about 300 functions of the Excel formula.
<iframe width="560" height="315" src="https://www.youtube.com/embed/QKqGMYdK_C8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Go to **Lessons** and open **Excel-like Formulas**. Either you can follow on screen instructions or the steps mentioned below:

1. Select a cell range in the listview. Right-click and select **Insert** to insert a column.
2. Select cell range of the inserted column and click on the **Merge Cells**.
3. Input column header name as required.
4. Input formula in the formula bar just like Excel.
5. Click on **✓** to validate the complete formula.
6. The column row will display this formula. Right-click and select **Format Cells** for formatting.
7. Choose the required settings under various options and click on **Ok** to apply. <br/> (This step is not a mandatory step, follow when it requires).
8. Click on **Home**->**Start** to check the result in the web browser. 

## Export To Excel
Learn to export page or listview to the Excel file.
<iframe width="560" height="315" src="https://www.youtube.com/embed/Es3ax2GEy48" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Go to **Lessons** and open **Export To Excel**. Either you can follow on screen instructions or the steps mentioned below:

1. Select cell range outside the listview.
2. Select **Button** cell type.
3. Input name of the button such as Export; Export to Excel, etc.
4. Go to **Cell Type** (right pane)->**Commands**.
5. Select **Export Listview To Excel** command and click on **Ok**.
6. Click on **Home**->**Start** to check the result in the web browser. 

## Query Data
learn to insert search and filtering criteria on webpage.
<iframe width="560" height="315" src="https://www.youtube.com/embed/851ks25lFF8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Go to **Lessons** and open **Query Data**. Either you can follow on screen instructions or the steps mentioned below:

1. Select cell range.
2. Select **Combo Box** cell type. 
3. Go to **Cell Type** (right pane)->**List Items** to define drop down list. 
4. To get items from existing data table, select the **Get items from data table** checkbox.
5. Select data table to pull data in list items.
6. Select **Value Column** and **Display Column**.
7. Select another cell range.
8. Select **Button** cell type and input button name.
9. Go to **Cell Type** (right pane)->**Commands**.
10. Select **Query Table** command and click on the **New Condition**.
11. Define condition(s) and click on **Ok** to apply.
12. Click on **Home**->**Start** to check the result in the web browser. 

## Publish To Server 
The lesson is about publishing the application on the server.
<iframe width="560" height="315" src="https://www.youtube.com/embed/tcN9D3-5W0o" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Go to **Lessons** and open **Publish To Server**. Either you can follow on screen instructions or the steps mentioned below:

1. Click on **Publish** tab.
2. Click on **Server** to open **Publishing Settings** window.
3. Input valid details and click on **Publish** button.
4. **Server Manager** will open.
5. Go to **Apps** tab and locate the application.
6. Click on its **Browse** button to open the application webpage. 

## Create Master Details
The lesson is about creating a webpage with List view of Orders  by linking with Table fields and then filtered view with Order Details.
<iframe width="560" height="315" src="https://www.youtube.com/embed/bhdVh8BNZ7w" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Go to **Lessons** and open **Create Master Details**. Either you can follow on screen instructions or the steps mentioned below:

1. Open **Estimates** page and select cell range from A20 to I35.
2. Click on **Insert Listview** in **Listview** tab.
3. Select Orderdetails table and click on OK.
4. Select first column and go to **Binding**
5. Select **Product ID** in **Binding Field**
6. Select **Add relation to the field in other table** to create a relationship to a field in other table.
7. Select **ProductName** in the **Display Field**.
8. Similarly, click on next column and select **Qty** in **Binding Field**
9. Click on third column and select **Rate** in **Binding Field**
10. Click on **Home**->**Start** to check the result in the web browser.

Learn to create the Listview with details in below steps:
11. Click and select the complete listview on **Estimate** page.
12. Click on the **Design** tab.   
13. Click on **Set Detail Listview**. **Detail Listview Settings** popup window will appear.
14. Select **OrderID** in **Select a related column of the detail listview**.
15. Select **Orders** master listview.
16. Click on **Ok**.
17. Click on **Home**->**Start** to check the result in the web browser.

## Calculated Fields
The lesson is about creating a webpage with a table having a calculated field by adding a source formula. There are two types of formula in **Forguncy**:
- **Inline Formulas** that can set more number of functions as compared to **Data Source Formulas**.
- **Data Source Formulas** that can be used for sorting, query, and statistics of Data. 
<iframe width="560" height="315" src="https://www.youtube.com/embed/VVPW66aC4R8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Go to **Lessons** and open **Calculated Fields**. Either you can follow on screen instructions or the steps mentioned below:

1. Right click on **orders** table and select **Add Calculated Field**.
2. Rename **Column Name** as **OrderMonth**.
3. Input formula in **Formula** field as **YEAR([OrderDate])&"/"&MONTH([OrderDate])**.
4. Click on **Ok**.
5. Go to **orderListing** page and click on **Ship To Address** column.
6. Go to **Binding** and select **OrderMonth** in **Binding Field**.
7. Click on **Home**->**Start** to check the result in the web browser.

## Aggregated Fields
The lesson is about creating a webpage by adding statistic formula field in an existing table.
<iframe width="560" height="315" src="https://www.youtube.com/embed/cr8_GeHP-xs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Go to **Lessons** and open **Aggregated Fields**. Either you can follow on screen instructions or the steps mentioned below:

1. Select a blank cell and input **Statistics** in the **OrderListing** page.
2. Select **Hyperlink** Cell Type.
3. Go to **Cell Type** (right pane) and click on **Commands**
4. Select **Page** as **New Page** and click on **Ok**.
5. Open **Statistics** page and select cell range from **B2 to O15**.
6. Select **Insert listview** and then select **OrderDetails** table.
7. Click on **Ok**.
8. Select cell range from **B3** to **H3** and then go to **Binding**.
9. Select **OrderID** in **Binding Field**.
10. Select **Add relation to the field in other table** to create a relationship to a field in other table.
11. Select **OrderMonth** in **Display Field**.
12. Right-click on **OrderDetails** table and select **Add Aggregated Field**.
13. Rename **Column Name** as **Total**.
14. Select **Aggregated Function Name** as **SUM** and **Amount** as **Data Column Name**.
15. Click on **Ok**.
16. Select another cell range from **I3** to **O3**.
17. Select **Total** as **Binding Field**.
18. Right click on the **Total** column and select **Format Cells**.
19. Select **Currency** in **Category** and click on **OK**.
20. Click on **Home**->**Start** to check the result in the web browser.

## Charts
The lesson is about adding a chart for the listview that you have created.
<iframe width="560" height="315" src="https://www.youtube.com/embed/Hpf1MVN_3aQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Go to **Lessons** and open **Charts**. Either you can follow on screen instructions or the steps mentioned below:

1. Select the listview for which you want to add chart.
2. Go to **Insert** tab->**Column**.
3. Click and select the chart.
4. You can change the chart's location, resize width and height similar to excel.
5. For this, edit width and height in the **Format** tab. 
6. Click on **Home**->**Start** to check the result in the web browser.
