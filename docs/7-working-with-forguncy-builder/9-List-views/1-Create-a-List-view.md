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
- Select cell range on the page for the list view area. It should be large enough to accomodate table data.
- Drag and drop the data table from the navigation window to the selection area *or* 
  Go to **Home** > **Insert Listview** and select the required table. 

Note: You can also set the list view area by selecting a cell and clicking [Home] → [Set as List View].
{:.note}

- Adjust the cell width according to the fields you want to display in the row template using [Merge Cells] etc. In addition to the method of merging cells in advance, you can also automatically merge cells by selecting a range with the mouse and directly dragging and dropping the table fields there. You can also adjust the size of cells by changing the width of columns and the height of rows in the same way as in Excel.
- Drag and drop the fields you want to display from the navigation pane onto the row template. Click [ ] next to the table name in the navigation window to display the field name. This field becomes the column.
- Sets the row template display format. The field data is displayed in the display format set in the row template.
- Click [Home] → [ (Debug)] to check the display.

## Specify details in list view settings

Set the list view display, behavior, etc.
- Right-click the list view to be set and click [List view settings] from the context menu, or double-click the preview display area of ​​the list view to open the setting dialog. Alternatively, select the list view and click the [ ] icon for either [List view style options] or [Update process] on the List view tool [Design] tab .
- The List View Settings dialog has four tabs: Appearance, Update & Select, Other Behavior, and Data. You can restore the default settings by clicking [Reset].

#### Appearance tab

Set the appearance, such as the presence or absence of headers and borders. If the number of data rows to be output to the exported list view area is small and blank areas occur, by enabling this check option, blank rows with the same style (ruled line, background color, etc.) as the template row will be created. Add to blank space. Empty rows that are added include formulas and summary fields, but no row header numbers are added. The operation of this check option is valid only for the results of Excel/PDF export, and does not affect the display on the web browser. Default is disabled.

#### Update & Select Tab

Set operations such as update processing and selection in the list view.

#### Other Actions] tab

Configure settings such as actions and focus movement when column headers are clicked.

#### Data] tab

Set the timing of fixing list view data.

Tip: Data extraction and sorting in the list view can be performed even when [Do not update list view data immediately] is enabled.
{:.note}
