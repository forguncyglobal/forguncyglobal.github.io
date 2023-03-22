---
layout: default
title: Text Box
parent: Cell Types
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Cell-types/text-box/
nav_order: 4
---

# {{ page.title }}

Setting the cell to the text box type allows to enter text. 

Select a cell/cell range and choose **Textbox** from the cell type drop-down list.

![Text-box](/assets/images/product-images/textbox-celltype.png)
{:.dropshadow}

Select the button and go to the **Cell Type** navigation pane, see below Table for the detail:

![Text-box-settings](/assets/images/product-images/textbox-celltype-settings.png)
{:.dropshadow}

|Features|Descriptions|
|:--|:--|
|Commands..|Sets the command to be executed when the value changes. The command is executed only when the focus leaves the text box or when the Enter key is pressed. See the [command](http://localhost:4000/develop/commands/#commands) for more information.|
|Data Validation..|Allows setting up data validation to restrict the entry of invalid data.|
|Set UI Permissions..|Allows you to do enable/ visible/editable settings.|
|Default value|Sets the default value of the text box. For example, if the default value is “A001” the text box will display “A001” as default text. You can also enter a formula. The result of the formula is displayed as a default value of the text box.|
|Show as Password| When **Show As Password** is checked, the entered characters will be displayed as ************|
|Unique in the bound data field| When **Unique in the bound data field** is checked, the value must be unique in the data field it is bound to.|
|Watermark|The prompt text that is displayed when there is no content in the text box for example: "Please enter text".|
|Icon|Sets the icon for the text box. Click **Select Image..** to select the icon for the button. You can select the built-in icon, or a local image in .jpg/.jpeg/.png/gif/.ico.bmp/svg format.|
|Read only|When checked, the text box is converted into a non-editable field.|
|Select text content on focus|When checked, all the text box content gets selected, and you can edit the content directly.|

