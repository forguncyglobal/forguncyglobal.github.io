---
layout: default
title: How to Use Pivot Table Cell Type
parent: Pivot Tables
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Pivot-tables/how-to-use-pivot-tables/
nav_order: 1
---

# {{ page.title }}

A pivot table is provided as one of the cell types. Pivot table cell type needs to use a list view as the source data. The steps to use pivot table cell type assuming that there is a list view are explained below. 

Note: The list view, which is the source data, does not necessarily have to be displayed on the screen at runtime.
{:.note}

### Steps to Create a Pivot Table

- Select the cell area and choose **Pivot Table** cell type.
- Select pivot table and go to **Pivot Table Settings** available in the right-pane-> *Cell Type* tab. You can also double-click on the pivot table to display the **Pivot Table Settings** dialog.
- In the **Pivot Table Settings** dialog, select list view, and drag and drop fields (that you want to add in pivot table) in *Columns*, *Rows*, and *Values*.
- Select **Field Settings** from the *value* field drop-down list.
- Select *Aggregated Value Fields* and *Total Summarized*. 

The types and contents of aggregation that can be used are as follows:

|Aggregation Method|Explanation|
|:--|:--|
|SUM|sum of values|
|AVERAGE|Numeric mean|
|COUNT|Number of data values|
|COUNTUNIQUE|Number of unique data values|
|MAX|Maximum value|
|MIN|Minimum value|
|FIRST|The first data displayed in the list view|
|LAST|The last data displayed in the list view|

- Click the **Number Format** button on the lower left to display the **Field Setting Format** dialog. Select suitable format and click the **OK** button.
- Also, click the **OK** button on the Pivot Table Settings dialog to apply the selection.
- Click **Style Settings..** from the right pane to open **Style Settings** dialog.
- In the **Style Settings** dialog, set both Column Width and Row Header Column Width to *AutoFit* and click **OK** to close the Style Settings dialog.
- Go to **Home** ribbon tab and click **Start** to debug. 


## Conditional Formatting in PivotTables

You can set conditional formatting for each of the *data area*, *subtotal area* and *total area*. Refer [Conditional Formatting in List View](https://docs.forguncy.net/working-with-forguncy-builder/List-views/Conditional-formating-in-list-view) for the details.