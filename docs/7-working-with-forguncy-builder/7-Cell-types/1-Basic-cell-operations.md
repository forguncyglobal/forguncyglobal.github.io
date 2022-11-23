---
layout: default
title: Basic Cell Operations
parent: Cell Types
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Cell-types/Basic-cell-operations/
nav_order: 1
---

# {{ page.title }}

Forguncy builder is similar to Excel. The pages consists of cells, similar to Excel sheets.
Home menu in the ribbon allows various settings for the cells.

![home-menu-settings](/assets/images/product-images/home-menu-settings.png) 
{:.dropshadow}
---

- [Basic operations](#basic-operations)
- [Right-Click Menu Operation](#right-click-menu-operation)

## Basic operations 
### Clipboard 
The clipboard area allows copy, paste, cut, and format cells. You can perform special paste operations such as paste only formulas, values, formats, commands, or all by expanding **Paste** (click the drop-down button)

### Font
allows to set the font, font size, bold, italic, underline, border, fill color, font color, and more.
 
### Alignment
Allows to set the alignment of text, increase or decrease indentation, wrap lines, and merge cells.
 
### Cell type
Allows to set the cell type such as buttons, text box, check box, radio button, hyperlink, combo box, number, date, image, and more for the cell. Click the drop-down button to view all cell types.
 
### Number
Allows cell formatting. You can set numbers, do alignment, change fonts, edit borders, and choose backgroud colors. The various number formatting categories available in the dialog box are as follows:

#### Table: Different Number Formatting 

|Format|Description|
|:--|:--|
|**General**|The default cell format. It has no specific number format. The general format rounds off the number with a decimal point and uses exponential notation if the cell is not wide enough to display large numbers like 12 digits or more.|
|**Number**|Used for a general representation of numbers. You can specify the number of decimal places to use, whether to use the thousands separator and how to display negative numbers.|
|**Currency**|Used for general monetary values. You can specify the number of decimal places to use, currency symbol, and how to display negative numbers.|
|**Accounting**|Also used for currency values.It helps in aligning decimal points in a column.|
|**Date**|Displays the date and time serial number as a date values based on the type and location selected.|
|**Time**|Displays the date and time serial number as a time values based on the type and location selected.|
|**Percentage**|Multiplies the cell value by 100 and displays the result with the percent symbol (%). Here, you can specify the number of decimal places to use.|
|**Fraction**|Displays numbers as fractions based on the selected fraction type such as Upto one digit (1/4), as half (1/2), etc.|
|**Scientific**|Displays numbers in exponential notation, replacing some of the digits with E+n. E (for exponent) refers to multiplying the preceding number by the nth power of 10. For example, the Scientific Count format for 2 decimal places displays 12345678901 as 1.23E+10, which is a 10-step power of 1.23 multiplied by 10. You can specify the number of decimal places to use.|
|**Text**|The cell is displayed exactly as entered. Cell content is treated as text even when a number is in the cell.|
|**Special**|Displays numbers based on the type and location selected. Useful for tracking list and database values.|
|**Custom**|Enables you to modify a copy of an existing numeric format code. Use this format to create and add a custom number format to the list of number format codes.|

### Find & Replace

You can search and replace strings and numbers. Advanced search options allow you to narrow down the searches, such as limiting the search to cells or list views.
![Find](/assets/images/product-images/find.png)
{:.dropshadow}

![Replace](/assets/images/product-images/replace.png)
{:.dropshadow}

- Click **Find and Replace** on the Home tab, or press Ctrl + F.
- Go to **Find** tab to search, and **Replace** tab to replace.

|**Character string to search**|Enter the character string or number you want to search. Alternatively, click the down arrow on the far right to select from the recently searched list|
|**Character string after replacement**|Enter the replaced character string or number. Alternatively, click the down arrow on the far right to select from the recently replaced list|
|**Within**|"Where" you want to search. It could be within current page or whole project.|
|**Find All**|Search item within the area defined. Click the search result from the list to jump to the referenced position|
|**Find Next**|Jump to the next found item (result) location. Click again to jump to next item and so on.|
|**Replace all**|Search for items on the page and replace all of them at once with the "Replace With" item.|
|**Replace**| Search for items on the page and replace them with the required value (one at a time). Click Replace again to search for more and replace.|

Perform **Advance search and replacement** action by clicking on **Option >>**

- Select target location for the search.
- Select serach direction as **Row** or **Column**.
- Select target to narrow down the search target range.
- Select **Case Sensitive** to make case-sensitive serach.
- You can search for cells that have exactly the same content or using regular expressions. 

![search results](/assets/images/product-images/Find-and-replace-search-results.png)
{:.dropshadow}

- Search results are displayed at the bottom of the screen.
- Double-click on the result to jump directly to the referred location.

## Right-click Menu Operation
Select a cell and right-click to perform operations like Cut, Copy, Paste, New Note, Format cells, and Find References.

![right-click-cell-menu-operations](/assets/images/product-images/right-click-cell-menu-operations.png)
{:.dropshadow}
 
### Add A New Note
You can add notes/comments/ instructions to the selected cell in an organized manner without changing page layout.
- Select a cell or range of cells
- Right-click and choose **New Note** option or press **Shift+F2** to open an editor window. 
- Enter a note.

![cell-note](/assets/images/product-images/cell-note.png)
{:.dropshadow}

- A small red triangle appears on the upper-right corner of the cell after adding a note. 
- A note for the cell appears on hovering the cell.
- You can edit and delete a note by right clicking on the cell.
 
### Format Cells
Opens cell formatting dialog box. You can set numbers, do alignment, change fonts, edit borders, and choose backgroud colors.

![Format-cells](/assets/images/product-images/format-cells.png)
{:.dropshadow}

