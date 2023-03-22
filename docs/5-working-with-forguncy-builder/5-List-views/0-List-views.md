---
layout: default
title: List Views
parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/List-views
nav_order: 5
has_children: true
has_toc: true
---

# {{ page.title }}

## Description

List views are used to list the data stored in a table and to identify the current record of a table used. For example, you bind a textbox to a field in a table. Now, to display the values of that current record in a text box you can create a list view.

Note: Current Record is one data for which a cursor exists in the target table data and is determined by the user which is used in various data binding operations.
{:.note}

In transitions of pages, i.e. between a list view page and a destination page having cells of the same table used, the current record code gets inherited by default. No need to create a new list view on the destination page to identify the current record.

List View Area is the list view display area and the *Second row* cells are called **Row Templates** that specify fields and bind table data.

![listview-insert-table](/assets/images/product-images/listview-insert-table.png)
{:.dropshadow}

To bind data field, drag and drop the field from the navigation pane onto the row template. Row templates fields width is column widths where data is displayed. Specify a sufficient width by merging cells, so that the data can be displayed. If you hide the column headers, the cells in the first row will become the row template. 

A column header is a string that is used as the header row of a table. This string and appearance of column header is editable.
Left edge of list view area can also be set as the row header, and this is editable.

Kindly refer [Working with Database](https://docs.forguncy.net/working-with-database/#working-with-database) to know more about database and table creation in Forguncy.


<!--
## List Display
You can list data by binding a table to a list view.

## Identify records

It binds the table to list view that uses identified records and helps in identifying records for the page in current record.


For example, if there are two sets of data in a table as shown in the figure below, it is not possible to determine whether to display the data of *Taro Yamada* or *Hanako Suzuki* records just by binding them to the table in a cell. If you can't determine, Forguncy won't show either data.
In such cases, you can arrange a list view so that the data for the record selected in the list view can be displayed. 

Selected records are carried over by page transitions and you can make selections on the crossing pages.

Selected record data is displayed on the destination page before the page transition. It can be disabled when it cross pages. For details, refer **Page transition**.

-->