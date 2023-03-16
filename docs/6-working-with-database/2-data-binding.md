---
layout: default
title: Data Binding
parent: Working with Database
permalink: /rworking-with-database/data-binding/
nav_order: 2
---

# {{ page.title }}

In Forguncy, Data binding refers to the association between page cells and table fields in order to display or update table data on the page.
Data binding can be set for page cells and the cells on listview row templates.

![data-binding](/assets/images/product-images/data-binding.png)
{:.dropshadow}

Data binding allows you to view, add, update, and delete table data through the cells on the page.

To display data in a cell on the page using data binding, it is necessary to select which record to display (determine the current record) among the multiple records that exist in the table. 

Note: To display the data in the table on the page without using data binding, there is a way to use " OData " function or　custom JavaScript .
{:.note}

If you bind data to the cells on the list view row template, you can display the data in the table on the page without any other settings. Use query commands to narrow down (search) the records to be displayed.　

After data binding to the cells on the page, use the [Update Table Data command](http://working-with-forguncy-builder/commands/Client-side-commands/update-data-table#update-data-table).

Note: Use custom JavaScript to update the data in the table without using data binding.
{:.note}

## Associating Table Data by Drag and Drop

You can combine data by dragging and dropping table fields. Here is an example of binding data to a cell-type text box.

- Create a text box.

![data-binding-text-box](/assets/images/product-images/data-binding-text-box.png)
{:.dropshadow}

- Expand the table fields.
- Display the fields of the table in the Navigation Pane and drag and drop the field to be concatenated into the text box.

![data-binding-drag-and-drop](/assets/images/product-images/data-binding-drag-and-drop.png)
{:.dropshadow}

- Check the binding of the data in the **Binding** on the right pane.

![data-binding-field](/assets/images/product-images/data-binding-field.png)
{:.dropshadow}

## Associating Table Data in the Data Binding Tab

You can view and edit table data by associating page cells with table fields. Here is an example to add data entered on a page to a field in a table.

- Create a new table and name it as *Employee Name*. 
- Create a button cell type on the page and name it as *Add*.
- Go to **Command** in **Cell Type** on the right pane and set the command to be executed when the button is pressed.
- Create a text box cell type and concatenate the *Name* field of the table *Employee Name*. Refer the below images:

![data-binding-update-table-data](/assets/images/product-images/data-binding-update-table-data.png)
{:.dropshadow}

![data-binding-update-table-data-settings](/assets/images/product-images/data-binding-update-table-data-settings.png)
{:.dropshadow}

- Go to **Home** and click **Start** to debug. 
- Enter employee name.

![data-binding-debug](/assets/images/product-images/data-binding-debug.png)
{:.dropshadow}

- Allow changes to sync and check table data for the update.

![data-binding-data-sync](/assets/images/product-images/data-binding-data-sync.png)
{:.dropshadow}
