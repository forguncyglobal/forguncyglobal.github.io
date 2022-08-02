---
layout: default
title: Radio Group
parent: Cell Types
grand_parent: Develop
permalink: /develop/Cell-types/radio-button/
nav_order: 8
---

# {{ page.title }}

The **Radio Group** cell type allows you to create multiple radio buttons.

![radio-group-celltype](/assets/images/product-images/radio-group-celltype.png)
{:.dropshadow}

Steps to create a radio group with cell type:
- Select a cell and go to **Radio Group** drop-down list. Multiple radio buttons are created in the selected cell and become a radio group type. You can arrange radio buttons horizontally or vertically. Merge cells or adjust cell widths to accommodate radio buttons.
- Configure radio groups in the right pane. Click on the **Cell Type** tab at the bottom of the right pane for radio group settings. The controls are as follows:

![radio-group-celltype-layout](/assets/images/product-images/radio-group-celltype-layout.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|Commands..|Sets the command to be executed when the value changes. See the [command](http://localhost:4000/develop/commands/#commands) for more information.| 
|Set UI Permissions..|Allows you to do enable/ visible/editable settings.|
|Default Value|Specify the value you want to display in the selected state. You can also use formulas. <br/>Note: Not applicable for List View.|
|Layout|Specifies the orientation of the radio buttons- *Vertical*/*Horizontal*.|
|list item| Specifies the text that appears to the right of the radio button. <br/> If you uncheck **Get items from data table**, you can manually set the items names in the text boxes below it. Use **+** and **-** to add or remove radio group items.<br/> Click on **Advanced..** to specify the value to be displayed in each radio button i.e. Display Value and the value used in formulas and data concatenation i.e. Value separately. <br/> ![radio-group-celltype-layout](/assets/images/product-images/layout-advance-settings.png) <br/> If you check **Get items from data table**, you can get the value to be displayed and the value from the field of the table. When the data in the table changes, it is automatically reflected in the list items. <br/> ![radio-group-celltype-layout](/assets/images/product-images/radio-group-celltype-list-items-data-table.png) <br/> Select **Add empty item** to add empty list item in the radio group. You can also specify the text in **Empty item text**. <br/> You can set query conditions by Data Query. <br/> Note: You cannot use Query Criteria in List View. <br/> By clicking **Sort Order**, you can set the conditions for how to sort and display at runtime. Check **Add an item "Other"** to display *Other* as an item and allow the user to enter a value in the text box. You can specify the width of the text box for input in pixels. The default value is 10. It cannot be used when **Style** is *Toggle* or *Button*. <br/> If you use related fields, the table associations must be between tables in the same database and in the same instance. For example, if you have an association between Forguncy's internal database and an external database such as SQL Server or Oracle Database, or if the databases are different and the instances are not the same between SQL Servers, the related fields cannot be used.|
|Same width for all items|This setting is displayed for **Horizontal** layout. If checked, all items will be displayed with the same width as the item with the longest string, regardless of the length of the item string. <br/> Note: This setting is reflected only at run time, and there is no change in the display at design time. This functionality is not applicable for list view.|
|Column Count|This setting is displayed for **Vertical** layouts. The items are automatically wrapped and displayed so that the number of columns matches with this setting value. Note: This setting is reflected only at run time, and there is no change in the display at design time. This functionality is not applicable for list view.|
|Margin between items|Specifies the margin between radio buttons (in pixels).|
|Style|Allows you to choose from four options: *System, Modern, Toggle,* and *Button*. The default value is *Modern*.|
|Primary Color|Specifies the fill color of the radio buttons. It is not applicable for *System* type style.|
|Secondary Color|Specifies the center circle of the selected radio button. It is not applicable for *System* type style.|
|Read only|If checked, user cannot make changes to the state of the radio buttons i.e. radio button is in non-editable format|

<!-- |Show cell type only in edit mode|If you remove the check, the radio button will be displayed even when not editing. This item can only be set in cell types on the list view.| -->
- Data concatenation can be performed when necessary. To concatenate data use two radio groups to narrow your options. When you select a value in Radio Group A, you can use Query Criteria to display only the choices related to that value in Radio Group B. 

    Steps are:
    - Create a table and then two radio groups.
    - Set the cell type to display the country name in the first radio group.
    - Set the second radio group to display the city name and click Query Criteria.
    - Set the query conditions as follows. Set the Country field values ​​to be filtered by the values ​​in the first radio group. If you select a country name in the first radio group, the city name will be narrowed down by that value and displayed in the second radio group.

Note: List view does not support this feature.
{:.note}