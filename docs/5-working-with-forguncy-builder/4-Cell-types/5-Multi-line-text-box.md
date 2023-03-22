---
layout: default
title: Multiline Text Box
parent: Cell Types
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Cell-types/Multiline-text-box/
nav_order: 5
---

# {{ page.title }}
Setting up a cell to the multiline text box type allows multi-line text input. It can hold multiple characters. Suitable for entering comments, feedback, etc.
Note: When typing in a multi-line text box, you can wrap a line with the Alt+Enter key combination.

Select a cell range and choose **Multiline Text** from the cell type drop-down list.

![Multiline-text-box](/assets/images/product-images/multiline-celltype.png)
{:.dropshadow}

Select the multiline text box and go to the **Cell Type** navigation pane, see below Table for the details:

![Multiline-text-box-settings](/assets/images/product-images/multiline-celltype-settings.png)
{:.dropshadow}

|Features|Descriptions|
|:--|:--|
|Commands..|Sets the command to be executed when the value changes. The command is executed only when the focus leaves the text box or when the Enter key is pressed. See the [command](http://localhost:4000/develop/commands/#commands) for more information.|
|Data Validation..|Allows setting up data validation to restrict the entry of invalid data. |
|Set UI Permissions..|Allows you to do enable/ visible/editable settings.|
|Default Value| Sets the default value of the Multiline text box. For example, if the default value is “A001” the text box will display “A001” as default text. You can also enter a formula. The result of the formula is displayed as a default value of the text box.|
|Watermark|The prompt text that is displayed when there is no content in the text box <br/> *For example*: "Please enter text".|
|Read only|If checked, user cannot make changes to the state of the multiline text box.|
|Select text content on focus|When checked, all the text box content gets selected, and you can edit the content directly.|
