---
layout: default
title: Repeater
parent: Cell Types
grand_parent: Develop
permalink: /develop/Cell-types/Repeater/
nav_order: 27
---

# {{ page.title }}

A repeater is a cell type that repeatedly displays a template for the number of data items in the list view to lay out separately from the page. In addition to vertical and horizontal display directions, it also supports the wrapping of template. The repeater allows data editing. 

Repeater cell type must use a list view as the data source. The list view does not necessarily have to be displayed on the screen at runtime. However, when exporting a page, do not create a list view in the area to the right or left of a repeater cell type. 

List views and repeater cell types are dynamically added according to the output data during the export process. If you place a listview or other repeater cell type to the right of a repeater cell type, it will affect the dynamic addition of rows and the resulting layout.

Steps to create a repeater cell type:

- Right-click the list view and select **Auto Set Column Names** from the context menu to set column names for all columns. 
![repeater_listview_contextmenu](/assets/images/product-images/repeater_listview_contextmenu.png)
{:.dropshadow}

- The repeater cell template requires column names because it does not bind directly to table fields. It binds with list view columns.
- Select an area of ​​cells and select **Repeater** cell type.
- Go to the **Cell Type** tab in the right pane and select the target list view in the **Select Listview** drop-down.
- Click the **Edit Template...** hyperlink to open the template editing screen. Here, you can set the layout of the template.

![repeater_cell_type_property](/assets/images/product-images/repeater_cell_type_property.png)
{:.dropshadow}

Note: The same operation can also be performed by right-clicking the repeater Cell type and select **Edit Template** from the context menu.
{:.note}

![repeater_edit_template](/assets/images/product-images/repeater_edit_template.png)
{:.dropshadow}

- If you want to design a template and display the list view data in the cell, set any column name in the **Related Column** field in the **Cell Type** tab (right pane).
- In addition to displaying data, you can also use input-enabled cell types.
- The dashed line displayed on the template sheet indicates the size of the repeater cell type on the parent page.
- Click the **Parent Page Snapshot** toggle button on the **Design** context tab of the **Template Page Tools** tab to edit the template while simultaneously viewing the state of the parent page. 
- Click the **End Edit Template** button on the Design contextual tab of the Template Page Tools contextual tab set to return to the parent page.

![repeater_edit_template](/assets/images/product-images/repeater_edit_template.png)
{:.dropshadow}

- If you click the **Start** button on the Home ribbon tab, you can see that the repeater template displays the bound data for the number of records in the list view and repeats.

![repeater_cell_type_output](/assets/images/product-images/repeater_cell_type_output.png)
{:.dropshadow}

Features that can be set on the **Cell Type** tab in the right pane of a repeater cell are:

![repeater_cell_type_property](/assets/images/product-images/repeater_cell_type_property.png)
{:.dropshadow}

|Property|Explanation|
|Select Listview|Select the list view that binds the data to the repeater cell type template. If the list view is not selected, the **Edit template..** will display an alert message. <br/> If there are listviews on the page, one of them will be automatically set.|
|Edit Template..|Switch the work pane to the template editing screen.|
|Display Mode|It supports three modes: <br/> -**Vertical**: Arranges the templates vertically in a single column. Only in this mode, the setting of the horizontal position of the cell is valid. <br/> -**Horizontal**: Displays templates horizontally in one line. <br/> -**Flow**: Displays the template wrapped at the end of the region.|
|Overflow Mode|Applicable only when Display Mode as *Flow* is selected. You can select *Overflow*, *Scroll*, or *Cut*. <br/> -**Overflow**: The repeater expands to fit the display size of the template to show all of its contents. <br/> -**Scroll**: A scrollbar appears on the repeater. <br/> -**Cut**: The template is displayed to the size of the repeater, and protruding part is not displayed.|
|Set content when there is no item..|Set the image and string to display when data does not exist. <br/> -**Image**: Sets the image to display in the repeater when no data exists. <br/> -**Image size**: Sets the size of the image in pixels. <br/> -**Text**: Sets the string to display in the repeater if no data exists. <br/> -**Orientation**: Horizontal option aligns the text to the right of the image and Vertical option places the text below the image. <br/> ![contentTo%20DisplayWhenThereIsNoItem](/assets/images/product-images/repeater_contentTo%20DisplayWhenThereIsNoItem.png)|

<!--
## Edit data
### Finalize data
The data finalization process differs depending on the [Data finalization timing] setting of the list view that is the data source of the [Repeater] type cell.
When [Do not refresh list view data immediately] is disabled
-If the current record in the list view is moved by clicking the area corresponding to each record on the repeater, the edited data will be reflected in the database.
-If you click outside the repeater's area, the data you were editing on the repeater at that point in time will be reflected in the database.
-If you set data validation rules for the input cells above the template, even if there is a validation rule error, the values ​​in the list view will be reflected in the display, but will not be reflected in the database.

When [Do not refresh list view data immediately] is enabled
-If you execute the [Update list view data] command whose [Processing type] is set to "Confirm list view update", all the data edited on the repeater will be reflected in the database.
-If the list view used as the data source of the [Repeater] type cell is set as a detailed list view, all data edited on the repeater will also be reflected in the database when the master data is confirmed.

## Data Validation Validation Behavior
If the data validation rule set in the input cell above the template is an error, the following commands will not be executed.
- [Update List View Data] command with [Process Type] set to "Confirm List View Update"
- Update Table Data command
- [Page transition] command

## Supplementary notes and notes
### Application design time
- f you copy and paste a Repeater cell type whose template has been edited, the edited contents of the template will not be copied. Note that this does not apply if the page is duplicated or imported from another Forguncy project.
- If you start debugging while the template editing screen is displayed in the task pane, the parent page of the template will be displayed if the start page is not set.
- The Delete Record command, normally available only for cells in listviews, is also available for cells in templates.
-If you copy a non-template cell such as a cell on the parent page and paste it on the template, the cell type will not be reflected, but only the style will be reflected. This is a behavioral design due to the limited cell types supported on templates.
- Templates don't support formulas, so the formula bar doesn't appear, but neither does typing formulas directly into cells or setting default values ​​to formulas.
- If the [Export to Excel (page)] command and [Export to PDF] are set to a [Button] type cell etc. in the template, only the template part of the record where the clicked button exists will be exported. At that time, the Excel file name will be the name that adds the record number to the "list view name". Note that parent pages cannot be exported.
- Regardless of the set value of [Allow editing] of the list view that is the data source of the list view that is the data source of the [Repeater] type cell, updating by the repeater is enabled.
- There is no way to add new data using a Repeater type cell. Consider using the Refresh List View Data command or the Refresh Table Data command.
- If you place a list view (including hidden columns) horizontally in a [repeater] type cell, the export process will not produce the expected results.
- If the [repeater] type cell part is hidden by the column hiding function or the row hiding function, the rows that are dynamically added by the data will not be hidden and will be output in the export result.

### Application runtime
- If the load on demand setting is enabled in the list view that is the data source of the [repeater] type cell, the load on demand function will work by scrolling the repeater's scroll bar to the bottom or right end.
- If you click the area corresponding to each record on the repeater, the current record of the list view will transition according to the clicked area.
-->