---
layout: default
title: Export Page to Excel
parent: Commands
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/commands/Export-page-to-excel/
nav_order: 9
---

# {{ page.title }}

This command exports the content of the pages to an Excel file.

![command-export-page-to-excel](/assets/images/product-images/command-export-page-to-excel.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|**Page**|Select page from the dropdown to export. You can export pages that are not displayed in the web browser to Excel, but if you set other than <Current page>, pages in the following cases will not be exported correctly. Such pages can be displayed in a browser and then exported to get correct results. A case where the settings related to the cell value are set in the "command at page load". If you export without actually loading the page on the browser, the "command at page load" will not be executed.|
|**Handling table overflow in excel**|Select *Add Rows* or *Overflow to Other Sheets* to set excel sheet for the page content. You can either add rows in the same sheet to adjust page content or add more sheets to export the page content.|
|**Excel Filename**|Select *Use page name*, *Use page title* or *Other* to specify the file name. <br/> In *Other*, you can use formulas. If the formula results in a N/A error, an error message will be displayed when the command is executed. <br/> If an invalid formula is used and the formula results in null, the page name will be used instead. If characters "\ / * ? " < >" that cannot be used in file names are used, all such characters are automatically replaced with "_".|
|**Formulas**|Exports calculated results of formulas as values ​to Excel and remove formulas. <br/> Even if this check option is not checked and both formula and data binding are set in the target cell, the value will be exported instead of the formula. <br/><br/> Note-This setting is valid only when *Current Page* option is selected.|

Read [Commands](https://docs.forguncy.net/working-with-forguncy-builder/commands/) to understand command execution steps.

- To set the Excel Page settings, use **Print Setup** dialog of **Print layout** tab.
- When you run the **Export Page to Excel** command on a master page, only the child pages displayed in the placeholder are exported to the Excel file.
- If a page other than *Current page* is selected in **Page**, the following pages will not be exported correctly. <br/> Such  page can be displayed correctly in a web browser and then can be exported to obtain correct results-

    - If you have set the cell value in pageload command and you export without actually loading the page on the web browser, the pageload command will not be executed.
    - If you have a cell reference such as "=A1" in the query that extracts the data to be displayed on the page. The value of a cell that references such a cell is determined only after it is displayed on the web browser. As a result, you will not get correct query results.
- The output result of the export differs depending on the cell type.
