---
layout: default
title: Date
parent: Cell Types
grand_parent: Develop
permalink: /develop/Cell-types/date/
nav_order: 12
---

# {{ page.title }}

You can enter the date directly or from the calendar with the help of this cell type. When you click **▼** of the date input, a calendar will be displayed to select the date.

![date_celltype](/assets/images/product-images/date_celltype.png)
{:.dropshadow}

![date_celltype_calendarinput](/assets/images/product-images/date_celltype_calendarinput.png)
{:.dropshadow}

Steps to create a Date cell type:

- Select a cell and go to the **Cell Type** drop-down list. 
- Select **Date** cell type. The selected cell becomes the date type. You can merge cells or adjust cell widths to fit the date digits.
- Go to the **Cell Type** tab at the bottom of the right pane to set the date input.
You can do the following settings from here:

![date_celltype_settings](/assets/images/product-images/date_celltype_settings.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|Command|Sets the command to run when the value changes. <br/> Note: This control has limitations in the list view.|
|Data Validation|Show/hide and enable/disable the cell type for respective the role. <br/> Note: This control has limitations in the list view.|
|Default value|Specifies the default value. You can also use formulas. <br/> Example: <br/> -If you write "=TODAY()", today's date will be displayed as the default value. <br/> -If you select "=TODAY()-1", the date of the previous day (yesterday) will be displayed. <br/>-If you select "=TODAY()+1", the date of the next day (tomorrow) will be displayed.|
|Date format|Sets the display format of date in the Edit mode. <br/> This field is not visible or configurable on mobile pages.|
|Show dropdown button|If checked, displays a calendar on the click of **▼**. It allows you to select and enter a date. <br/> This field is not visible or configurable on mobile pages.|
|Show calendar scrollbar|If checked, a scroll bar will be displayed on the calendar. You can scroll to the same month of the previous year or the same month of the next year.|
|Read-only|Makes the cell read only and user cannot enter or select dates.|
|Select text content on focus|All values ​​are automatically selected on the click of the cursor. <br/> Note: This control has limitations in the list view.|

- Data concatenation can be performd if required from the **Binding** tab at the bottom of the right pane.
