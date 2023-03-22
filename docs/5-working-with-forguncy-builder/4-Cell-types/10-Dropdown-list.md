---
layout: default
title: Dropdown List
parent: Cell Types
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Cell-types/dropdown-list/
nav_order: 10
---

# {{ page.title }}

This cell type allows you to create a dropdown list.

![dropdown_list_celltype](/assets/images/product-images/dropdown-list-celltype.png)
{:.dropshadow}

Steps to create a Dropdown list cell type:

- Select a cell, and go to the **Cell Type** drop-down list. 
- Select **Dropdown List** cell type. 
- Go to the **Cell Type** tab at the bottom of the right pane for the configuration.
You can do the following settings from here:

![dropdown_list_celltype_settings](/assets/images/product-images/dropdown-list-celltype_settings.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|Commands..|Sets the command to be executed when the image is clicked.|
|Data Validation|Show/hide and enable/disable the cell type for respective role. <br/> Note: This control has limitations in the list view.|
|List item|-Specifies the text to be displayed in the dropdown list. <br/> -Use **+ -** to increase or decrease items. <br/> -**Advanced..** allows you to specify the values ​​to be displayed in the dropdown list. <br/> -On checking **Get items from data table**, you can select data table, value column, and display column. <br/> ![dropdown_list_celltype_settings-listitems](/assets/images/product-images/dropdown-list-celltype_settings_listitems.png) <br/> Any changes to the data in the table are automatically reflected in the list items. <br/>You can enable **Add empty item** and define text to display as **Empty item text** <br/> You can set multiple items to be displayed in the drop-down list by clicking **Subitems..**. You can also specify items from other tables if you have set a table association <!-- (see "Creating a multi-column combo box" on this page) -->. <br/> The width of the drop-down list is usually the same as the width of the combo box cell. <br/>If the list has 1,000 rows or less, if the list has 1,000 rows or less, the column width will be automatically adjusted according to the item value, and the width of the drop-down list will change accordingly. if the list exceeds 1,000 rows, for performance reasons, the column widths are not automatically adjusted and all column widths are set to 100 pixels. <!--In order to avoid this phenomenon, use the load on demand function and make sure that the number of rows read for the first time does not exceed 1,000.--> <br/> **Data Queries** allows to set query conditions. It narrows down the selection of items in the dropdown list. <br/> **Sort Order** allows to set the sort criteria for the list items when retrieving data from the table.|
|Default Value|Specifies default values ​​for values ​​used in formulas, data bindings, and user input. You can also use formulas|
|Auto Filter|Displays items that match the value entered by user in the dropdown list. User can restrict search as by choosing *Match All*, or *Start With*. User can also choose *None* for free search.|
|Dropdown Button| Sets the display of the dropdown button ("▼" on the right side of the list) as *Always show*, *Hide*, and *Show on focus*. <br/> In the case of a dropdown list cell type set in the row template of the list view, even if this setting is set to "always display", the drop-down button will not be displayed when the application is executed because the cell is in an edit state when the cell is double-clicked. This field is not visible or configurable on mobile pages.|
|Watermark|Specify the watermark character to be displayed when not entered or not selected. This field is not visible or configurable on mobile pages.|
|Read-only|User will not be able to enter values ​​or change selections.|

- Data concatenation is performed as necessary.

<!-->
## Create a Multi-Column Dropdown List

You can display multiple columns in a dropdown list.

- Create two tables for master-detail relationship.
- Create a page and add a dropdown list.
- Go to **Cell type** (right-pane) and click on **Advanced..** below **List Item**. 
- Set the **Value Field** to *ID* of the *Detail* table and the **Display Field** to *Product*.
- Click "Drop-down list display items" and set as follows. Fields in the detail table can be changed by "Header Name".
- Set the display format of "price".
- Creates a combo box with multiple items displayed in a drop-down list.

Note: Multi-column dropdown list cannot be set on mobile pages.
{:.note}
-->