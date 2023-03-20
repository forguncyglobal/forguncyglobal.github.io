---
layout: default
title: Export Listview to Excel
parent: Commands
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/commands/Client-side-commands/Export-listview-to-excel
nav_order: 8
---

# {{ page.title }}

The command exports the content of the ListView to an Excel file. 

![command-export-listview-to-excel](/assets/images/product-images/command-export-listview-to-excel.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|**Select listview to export**|Select Listview from the dropdown list that you want to export into excel.|
|**Excel filename**|Select **Same as Listview name** or **Other** to specify the file name. <br/> In **Other**, you can use formulas. If the formula results in a N/A error, an error message will be displayed when the command is executed. <br/> If an invalid formula is used and the formula results in null, the listview name will be used instead. If characters "\ / * ? < >" that cannot be used in file names are used, all such characters are automatically replaced with "_".|
|**Formulas**|Exports calculated results of formulas as values ​to Excel and remove formulas.|

Read [Commands](https://docs.forguncy.net/working-with-forguncy-builder/commands/) to understand command execution steps.