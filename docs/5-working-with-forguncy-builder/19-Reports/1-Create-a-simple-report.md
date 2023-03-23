---
layout: default
title: Create a Simple Report
parent: Reports
grand_parent: Working with Forguncy Builder
permalink: /develop/reports/create-a-simple-report/
nav_order: 1
---

# {{ page.title }}

The steps to create a simple report are as follows:

- Go to **Create** tab and select **Page Report**.

![report-create](/assets/images/product-images/report-create.png)
{:.dropshadow}

- A new report page will appear.

![report-new-page](/assets/images/product-images/report-new-page.png)
{:.dropshadow}

- Right-click on the report in the navigation pane and select **Add Data Source** from the context menu. 

![report-add-data-source](/assets/images/product-images/report-add-data-source.png)
{:.dropshadow}

- Edit data source details in the **Edit Data Source** dialog. 

Selecting a target table will automatically load and display the fields from the database. You can add or delete coulmns as required.

![report-add-data-source-dialog](/assets/images/product-images/report-add-data-source-dialog.png)
{:.dropshadow}

- Edit the report:
    - Add a report control. Drag and drop a TextBox onto the page, double-click it and set its value as *Test Report*.

    ![report-edit-textbox](/assets/images/product-images/report-edit-textbox.png)
    {:.dropshadow}

    - Drag and drop the Table onto the page.

    ![report-edit-table](/assets/images/product-images/report-edit-table.png)
    {:.dropshadow}

    - Click the Table and move the mouse cursor to the left edge of the last column to display the column handles and click the plus sign to add more columns.

    ![report-edit-table-controls](/assets/images/product-images/report-edit-table-controls.png)
    {:.dropshadow}

    - Concatenate the data. Select a field from the data source by clicking the three dots to the right of each column in the second row .

    ![report-edit-table-concatenate](/assets/images/product-images/report-edit-table-concatenate.png)
    {:.dropshadow}

    - To adjust the size, select the entire Table and drag and drop the three control anchor points with the mouse to change the Table size.

    ![report-edit-table-anchor-points](/assets/images/product-images/report-edit-table-anchor-points.png)
    {:.dropshadow}

    - Select Table and set the table style in **Properties** on the right. The **Data** allows you to do data binding but you need to add a data source first.

    ![report-properties](/assets/images/product-images/report-properties.png)
    {:.dropshadow}

    ![report-data](/assets/images/product-images/report-data.png)
    {:.dropshadow}

    - Click the **Preview** button to preview the report. 

    ![report-preview](/assets/images/product-images/report-preview.png)
    {:.dropshadow}
    
    - You can improve the preview display speed of reports with a large amount of data by setting the **Record limit for AR preview in designer**. To do so, go to **File** -> **Options** and select **Application Settings**. 

    ![report-application-settings](/assets/images/product-images/report-application-settings.png)
    {:.dropshadow}

    - To set the report permissions, right-click on the report in the navigation pane and choose **Edit Report Permission..** from the context menu. 
    
    ![report-set-permission](/assets/images/product-images/report-set-permission.png)
    {:.dropshadow}

    Set report permission in the **Edit Report Permission** dialog box.

    ![report-set-permission-dialog](/assets/images/product-images/report-set-permission-dialog.png)
    {:.dropshadow}

    