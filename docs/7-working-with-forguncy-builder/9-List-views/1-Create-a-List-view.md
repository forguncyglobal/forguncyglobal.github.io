---
layout: default
title: Create a List View
parent: List Views
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/List-views/create-a-list-view
nav_order: 1
---

# {{ page.title }}

Steps to create a list view are-

- Create a data table to display in the list view.

![listview-table](/assets/images/product-images/listview-table.png)
{:.dropshadow}

- Select cell range on the page for the list view area. It should be large enough to accomodate table data.
- Drag and drop the data table from the navigation window to the selection area *or* 
  Go to **Home** > **Insert Listview** and select the required table. 

![listview-insert-table](/assets/images/product-images/listview-insert-table.png)
{:.dropshadow}

- Adjust the column width according to the fields you want to display by using **Merge Cells**. In addition to the method of merging cells in advance, you can also automatically merge cells by selecting a cell range with the mouse and directly dragging and dropping the table fields there. The table fields become the listview column.

Note: You can adjust the cell size by changing the width of columns and the height of rows in the same way as in Excel.
{:.note}

- Go to **Home** > **Debug** to run and check the display.

![listview-insert-table-output](/assets/images/product-images/listview-insert-table-output.png)
{:.dropshadow}

### Set the list view display, behavior, and more

![listview-setting](/assets/images/product-images/listview-settings.png)
{:.dropshadow}

Right-click the list view and select **List view settings** from the context menu, or double-click the preview display area of ​​the list view to open the setting dialog. 

The List View Settings dialog has four tabs-Appearance, Edit & Select, Other Behavior, and Data. You can restore the default settings by clicking the **Reset** button.

### Appearance Tab
Set the appearance, such as the presence or absence of headers and borders.

|Controls|Description|
|:--|:--|
|**Show Column Header**|If checked, show column headers. Default is Enabled. Specifies the number of rows to display in the column headers.|
|**Show Row Header**|Display row headers in the first column. Default is disabled.|
|**Show Selection Column**|Show selection columns. Default is disabled.|
|**Show Total Row**|Display summary rows. By default it is disabled. If you check this setting, the Show in first row check option appears. If the Show at top row check option is enabled, the summary row will be displayed at the top of the list view. Otherwise, it will be displayed at the bottom of the list view area. Default is disabled.|
|**Hide selection when focus is lost**|If the list view doesn't have the focus (when it's not active), it doesn't show the selection pane. Default is disabled.|
|**Show Edit status icon**|Displays an icon in the row header of each newly created record or record containing changes. Also, cells with changed values ​​are underlined. Default is Enabled.|
|**Show scroll bar only during operation**|If this setting is enabled, the scrollbar will be displayed only while operating the list view. For example, scrollbars appear when you edit a listview or when you move the mouse pointer over the listview. If this setting is disabled, scrollbars are always displayed. Default is Enabled.|
|**Add empty lines to blank areas, apply styles, and formulas**|If the number of data rows to be output to the exported list view area is small and blank areas occur, by enabling this check option, blank rows with the same style (ruled line, background color, etc.) as the template row will be created. Add to blank space. Empty rows that are added include formulas and summary fields, but no row header numbers are added. The operation of this check option is valid only for the results of Excel/PDF export, and does not affect the display on the web browser. Default is disabled.|
|**Autofill blank row**||

### Edit & Select Tab

Set operations such as update processing and selection in the list view.

|Controls|Description|
|:--|:--|
|**Allow editing list view**|Allows editing of data. This field is not visible or configurable on mobile pages. Default is disabled. |
|**Display delete button**|An **X** icon for deleting the record is displayed to the left of the line where the current record is set by selecting the line. Click the **X** icon to display a dialog to confirm the deletion. Default is disabled.|
|**Display newly added row**|A blank row appears at the bottom of the list view for new data entry. This field is not visible or configurable on mobile pages. Default is disabled.|
|**Always in edit mode**|When the focus moves to a cell, that cell automatically enters edit mode. This feature is only for cell types that can be edited with the keyboard. Default is disabled.|
|**Allow drag fill**|You can autofill by dragging the lower right corner of the cell as in Excel. In addition, since this function is effective only for areas where cells exist, it is not possible to continuously generate new lines while dragging with Autofill. This field is not visible or configurable on mobile pages. Default is disabled.|
|**Allow drag move**|Cells can be moved by dragging. This field is not visible or configurable on mobile pages. Default is disabled.|
|**Select unit by cell or row**|Sets the selection unit to cells or rows. The default is "cell". <br/> If you select "Row", you will see the "Do not automatically select first row when loading data or paging" check option. If this check option is not checked, the first row will be automatically selected when reading data or paging. Note that if this check option is checked, there will be no selected rows when reading data or paging, but the current record still exists. Also, if you don't show the selection column, once you've selected it, there's no way to unselect anything.|
|**Always keep selection rows**|It works effectively only when the "selection column" of the list view is checked. For details on the selected column, refer to Selected Column Display (List View). When this setting is enabled, the selected column will not be cleared when paging through list views that use [Page Navigation] type cells, but will be retained. Default is disabled. |
|**Don't select multiple cells or rows**|If you enable this setting, you will not be able to select multiple cells or rows. Cell or row depends on the selection units setting. Default is disabled. |
|**Insert**|When load on demand is enabled, the **Insert** menu is disabled.|
|**Duplicate**|Duplication with multiple rows selected is enabled only if the Do not update list view data immediately check option is checked.|
|**Delete**|Even if you select multiple lines and delete, only one line of the current record will be deleted.|

### Other Behavior Tab

Configure settings such as actions and focus movement when column headers are clicked.

|Controls|Description|
|:--|:--|
|**Column Header Behavior**|Sets the behavior on click of the column header. <br/> **Select whole column when clicked**- Click the column header to select the entire column. <br/> **Sort when clicked**- Each time you click a column header, the records are sorted alternately between ascending and descending order based on the value of that column. <br/> **Dropdown menu to sort and filter**- A dropdown for sorting and filtering is displayed on clicking the column header, similar to the column header filter in an Excel table. <br/><br/> *Note*- Settings other than **Select whole column when clicked** are valid only for columns for which data binding is set. The default value is **Dropdown menu to sort and filter**.|
|**List view gets focus when Tab is pressed**|If this setting is disabled, the list view will be skipped even if the focus is moved with the Tab key when the focus is on an element other than the list view. Default is Enabled.|
|**Cell's focus moves horizontally when enter is pressed**|If this setting is enabled and the Enter key is pressed while the focus is on a cell in the list view, the focus will move horizontally. Default is disabled.|
|**Freeze Panes**|If you create a horizontally scrollable list view using the Ignore Hidden setting, you can freeze any column from the top, or any column from the bottom, or both, and scroll horizontally.|
|**Auto-fit**|If **Auto-fit row height** is enabled, the row height will be automatically adjusted so that the contents of all cells in the list view can be displayed. <br/> If **Auto-fit column width** is enabled , auto-adjusts the width of the columns to show the contents of all the cells in the list view. <br/> Note that if the number of rows in the column header is two or more and the merging settings are different between the upper and lower headers, the contents of that header cell will not be automatically adjusted. <br/>The default value is disabled for both settings. <br/><br/> *Note*- If there is an empty column and **Automatically adjust column width** is enabled, the column size will be fixed and wider than usual. Normally, columns (blank columns) for which data binding or values ​​are not directly entered in list view columns are not displayed while the application is running. However, blank columns to the left of the column in which values ​​are set are displayed as blank columns. This also applies to blank columns to the left of the hidden column if the hidden column has a value.|

### Data Tab

Set the timing of fixing list view data.

