---
layout: default
title: Check Box
parent: Cell Types
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Cell-types/Check-box/
nav_order: 6
---

# {{ page.title }}

The **Checkbox** cell type allows you to create a checkbox. When the cell value is 0, it is in the unchecked state, and when it is 1, it is in the checked state. 
![chekbox-celltype](/assets/images/product-images/checkbox-celltype.png)
{:.dropshadow}

Note: The strings "0" and "1" are not supported.
{:.note}

Steps to create a checkbox with cell type:

- Select a cell and go to **Cell Type** drop-down list. 
- Select **Checkbox** cell type.This will convert the selected cell into a check box. 
- The text is displayed on the right side of the check box. Hence, set the cell width in such a way so that it can be displayed without merging the cells.
- Click on the **Cell Type** tab at the bottom of the right pane for checkbox settings. The controls are as follows:

![checkbox-celltype-tab](/assets/images/product-images/checkbox-celltype-tab.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|Commands..|Sets the command to be executed when the value changes. See the [command](http://localhost:4000/develop/commands/#commands) for more information.| 
|Set UI Permissions..|Allows you to do enable/ visible/editable settings.|
|Checked by default|By defalut, it is marked as checked. Check/uncheck will pass "True" and "False" value respectively.|
|Text|Allows you to specify the text to be displayed on the right side of the checkbox.|
|Style|Allows you to choose from four options: *System, Modern, Toggle,* and *Button*. The default value is *Modern*.|
|Primary Color|Specifies the fill color of the checkbox. It is not applicable for *System* type style.|
|Secondary Color|Specifies the color of the tick mark. It is not applicable for *System* type style.|
|Read only|If checked, user cannot make changes to the state of the checkbox i.e. checkbox will appear in non-editable format.|

Note: The above mentioned items cannot be set in the **Checkbox** cell type on the list view.
{:.note}
<!-- Data concatenation is performed if necessary. For information on how to concatenate data , see Concatenating data . -->