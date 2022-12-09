---
layout: default
title: Print/Export Page to PDF
parent: Commands
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/commands/Client-side-commands/Print-export-page-to-pdf
nav_order: 10
---

# {{ page.title }}

With this command, you can export the page content to a PDF file.

![print-export-page-to-pdf](/assets/images/product-images/command-print-export-page-to-pdf.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|**Page**|Specifies the pages to export. You can output to PDF a page that is not displayed in the web browser, but if you set other than <Current page>, pages in the following cases will not be exported correctly. Such pages can be displayed in a browser and then exported to get correct results. <br/> A case where the settings related to the cell value are set in the "command at page load". If you export without actually loading the page on the browser, the "command at page load" will not be executed.|
|**PDF file name**|Select *Use page name*, *Use page title* or *Other* to specify the file name. <br/> In *Other*, you can use formulas. If the formula results in a N/A error, an error message will be displayed when the command is executed. <br/> If an invalid formula is used and the formula results in null, the page name will be used instead. If characters "\ / * ? " < >" that cannot be used in file names are used, all such characters are automatically replaced with "_".|
|**Autofit row height**|Automatically adjusts the cell values such as- <br/> Numbers and Dates: Zoom Out to Fit <br/>Numbers and non-date strings: Expands the row height to accommodate strings. <br/><br/> Note- The wrap text must be enabled in **Format Cell** dialoge. Cells with vertical cell merging are not subjected to automatic adjustment. <br/> ![format-cell](/assets/images/product-images/format-cell.png)|

Read [Commands](https://docs.forguncy.net/working-with-forguncy-builder/commands/) to understand command execution steps.


<!--
## About Margins

The margins specified in "Export print settings..." create a drawing image with that area added when outputting to PDF. Note that they are not set as numerical values ​​for margins in Acrobat Reader. This is because the PDF itself is a file format that is created with a fixed layout and number of lines on a single sheet of paper, so the margins are set and output when the PDF is generated.
Even if the margin is set to 0, it may appear as if the margin is slightly added instead of being completely 0 in the PDF output. By unchecking the "horizontal" and "vertical" check boxes at the bottom of the margin setting screen, you can output with the margins completely invisible (screen drawing is done in pixels, (Since actual printing is done in physical units, this difference in scale creates this small margin.This checkbox is there to accommodate this difference in scale.)

If the data does not fit within the page and protrudes, Forguncy carries over to the next page in cell units and row units. In other words, for example, if there is a cell with a width of "25" and it does not fit "5", all "25" will be carried over to the next page, not "5". For this reason, even if it protrudes even slightly, it will be output as if it is larger than it actually is.

If you want to output to PDF at the very limit of the paper size, specify 0 for all margins, turn off the "horizontal" and "vertical" check boxes, and make the layout slightly smaller so that the entire image is drawn. should output

When printing on the Adobe Reader side, it is necessary to adjust the print settings on the Adobe Reader side before printing.

Note: <br/>To set the page settings for the output PDF, use the [Report] ribbon tab. For more information, see Export print settings. <br/><br/>If you run the Export PDF command on a master page, only the child pages displayed in placeholders will be exported to PDF files. <br/><br/> PDF files usually appear as new tabs in your web browser, but are affected by your web browser's pop-up blocker settings. For example, in the case of Google Chrome, if you try to open new tabs in succession by default, the second and subsequent tabs will be blocked by the pop-up blocking function. Also, on iPhone and iPad, Forguncy will redirect the current page to a PDF output instead of a new tab in your web browser. This is a workaround for Safari, the web browser on these devices, which also blocks popups on the first new tab.
{:.note}

-->