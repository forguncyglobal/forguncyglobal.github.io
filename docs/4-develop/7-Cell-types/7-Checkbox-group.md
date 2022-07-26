---
layout: default
title: Checkbox Group
parent: Cell Types
grand_parent: Develop
permalink: /develop/Cell-types/Checkbox-group/
nav_order: 7
---

# {{ page.title }}

The **Checkbox Group** cell type allows you to create multiple checkboxes. It can be in both vertical and horizontal format. 

![chekbox-group-celltype](/assets/images/product-images/checkbox-group-celltype.png)
{:.dropshadow}

Note: If you want to save the checkbox group data in a table, set the destination field to "text type". This is because the value of the selection items such as "Item 1, Item 2, Item 3" separated by commas is the value stored in the table field.
{:.note}

Steps to create a checkbox group with cell type:
- Select a cell and select [Checkbox Group] from the [Home] → [Cell Type] drop-down list. Multiple checkboxes are created in the selected cell to form a checkbox group type. You can place the checkboxes horizontally or vertically. Merge cells and adjust cell widths so that you can place checkboxes.
- Set the check box group in the right pane. Click the Cell Type tab at the bottom of the right pane to set the check box group.

![checkbox-group-celltype-tab](/assets/images/product-images/checkbox-group-celltype-tab.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|command|Sets the command to be executed when the value changes. See command (normal).|
|Cell access control|Show / hide the cell type and enable / disable it for each role. See Cell Access Control for more information. This item cannot be set in the cell type on the list view.|
|List item|Specifies the text to be displayed on the right side of the checkbox. <br/> - If you uncheck Get data from table, you can manually set the text from the text box below it. You can increase or decrease the check box items with [+] and [-]. ![checkbox-group-celltype-list-items](/assets/images/product-images/checkbox-group-celltype-list-items.png) <br/> -Click [Detailed Settings] to specify the value to be displayed in each check box (value to be displayed) and the value (value) used in formulas and data concatenation. <br/> If you check [Get data from table], you can get the value to be displayed and the value from the field of the table. When the data in the table changes, it is automatically reflected in the list items.<br/>![checkbox-group-celltype-list-items-data-table](/assets/images/product-images/checkbox-group-celltype-list-items-data-table.png) <br/> You can set query conditions by clicking Query Criteria ( see Query ). <br/> <br/> Note: You cannot use Query Criteria in List View. {:.note} <br/><br/> By clicking [Sort Criteria], you can set the conditions for how to sort and display at runtime. Check Add "Other" as an item to display "Other" as a choice and allow the user to enter a value in the text box. You can specify the width of the text box for input in pixels. The default value is 100. It cannot be used when [Style] is "Switch" or "Button". <br/> ![checkbox-group-celltype-list-items-other-item](/assets/images/product-images/checkbox-group-celltype-list-items-other-item.png) <br/> If you use related fields, the table associations must be between tables in the same database and in the same instance. For example, if you have an association between Forguncy's internal database and an external database such as SQL Server or Oracle Database, or if the databases are different and the instances are not the same between SQL Servers, the related fields cannot be used.|
|Default value|First, specify the values ​​you want to display in the checked state, separated by commas. You can also use mathematical formulas. This item cannot be set in the cell type on the list view.|
|Layout|Specify the placement direction of the check box. This item cannot be set in the cell type on the list view.|
|Display all items with the same width|This setting is displayed for "horizontal" layouts. If checked, all items will be displayed with the same width as the item with the longest string, regardless of the length of the item string. Note that this setting is reflected only at run time, and there is no change in the display at design time. This item cannot be set in the cell type on the list view.|
|Number of displayed columns|This setting is displayed for "vertical" layouts. The items are automatically wrapped and displayed so that the number of columns is the same as this setting value. Note that this setting is reflected only at run time, and there is no change in the display at design time. This item cannot be set in the cell type on the list view.|
|Margin between items|Specifies the margin between checkboxes (in pixels).|
|style|Choose from four options: System, Modern, Switch, and Button. The default value is "modern". This item cannot be set in the cell type on the list view.|
|Main color|Specifies the main color that is valid when the style is set to something other than "System". For example, in the case of "Modern", the fill color at the time of checking is the main color. This item cannot be set in the cell type on the list view.|
|Sub color|Specifies the main color that is valid when the style is set to something other than "System". For example, in the case of "Modern", the color of the check mark at the time of checking is the sub color. This item cannot be set in the cell type on the list view.|
|Read-only|It is read-only and cannot be clicked to change the state of the check.|
|Show cell type only in edit mode|If you uncheck it, the checkbox group will be displayed even when you are not editing. If unchecked, the [Default], [Layout], and [Display all items with the same width] settings cannot be used. This item can be set only for the cell type on the list view.|

Note: When you open a file created with an older version of Forguncy Builder, all "Show cell types only in edit mode" is unchecked.
{:.note}

- Data concatenation is performed if necessary. For information on how to concatenate data , see Concatenating data .