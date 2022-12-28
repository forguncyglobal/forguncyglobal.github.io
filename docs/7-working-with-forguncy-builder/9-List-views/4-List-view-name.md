---
layout: default
title: List View Name
parent: List Views
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/List-views/list-view-name
nav_order: 4
---

# {{ page.title }}

The list view has **List View Name** in addition to the cell name. Also, each cell in the template row has a column name. These names are used in custom JavaScript operations on the list view and in the Export to Excel List View command.

Steps to define list view and list view column names are-

## Define List View Name

- Select the entire List View. 
- Enter the list view name in one of the following ways: 
    - Enter from the **Cell type** tab in the right pane
    - Input from **List View Tools** -> **Design** tab

Note- The list view name is used as a parameter of the Page object's .getListView( name ) method when using JavaScript, and when selecting the target list view with the Export to Excel List View command.
{:.note}

## Column Name Definition

- Select a cell on the listview row template. 
- Click the row template details cell (not the list view header row).
- Click the **Cell Type** tab at the bottom of the right pane and enter a name in **Column Name**. This name will be the *Column Name* for each column in the list view.

Note- ListView column names are used as parameters *columnName part* of ListView object's .getValue( rowIndex, columnName ) and .setValue( rowIndex, columnName, value ) methods when using JavaScript. Cell names are not allowed in these methods.
{:.note}

## Automatic Setting of Column Names

- Select the entire List View.
- Right-click and select **Auto Set Column Names** from the context menu. 

Note- <br/>* If the row template cells are data bound or have some value or formula set, the header name will automatically be set as the column name. <br/> * If the value is set and the header name is not set, use the value as the column name. <br/> * If the formula is set and no header name is set, it will use the value "COLUMN" as the column name.
{:.note}


