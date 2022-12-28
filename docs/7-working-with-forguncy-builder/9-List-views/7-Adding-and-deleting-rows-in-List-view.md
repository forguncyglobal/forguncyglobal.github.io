---
layout: default
title: Adding and Deleting Rows in List View
parent: List Views
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/List-views/adding-and-deleting-rows-in-list-view
nav_order: 7
---

# {{ page.title }}

To add or delete rows in the list view, go to **Design** -> **Editing** and check the **Allow adding new rows** and **Display Delete Button** checkboxes.

## Where the Row will be added

New rows are added to the end of the list view by default.
The data displayed in the list view is basically displayed in the order of the records in the data-bound table. Adding a new line adds a record to the end of existing records, so a new line is also added to the end of the list view.

If the Row Header Context Menu setting is enabled, you can add a new row at any position by inserting a row from the row header context menu.

The list view can be sorted, so you can change the visual order. For example, provide a separate input field and add button on the page. By executing the "Update data table" and "Sort" commands with the button command for addition, adding data to the table and sorting the data on the list view in succession, can appear to have data appended to it.

## When list view values ​​are reflected in the database

The timing when the added or deleted value of the row is reflected in the database as a record is when the focus moves to another row. Until then, it is only displayed in the list view, and it is not reflected in the database. If you want the data to be reflected in the database when you click a button instead of when the focus moves to another row, right-click the list view and select "List view settings...", then on the "Data" tab, select "Update list view data immediately." and only update if" is checked.