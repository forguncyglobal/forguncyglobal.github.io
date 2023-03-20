---
layout: default
title: Features and Concepts
parent: Print Layout
grand_parent: Working with Forguncy Builder
permalink: /develop/Print-layout/features-and-concepts/
nav_order: 1
---

# {{ page.title }}

the functions and concepts that make up a report in order to understand the rules for Excel/PDF export to output based on

## Print size and coverage

The print size refers to the output range for one page when finally printed on paper. This area is determined by Margins, Orientation, Size, etc. on the Report tab. 

![print-layout](/assets/images/product-images/print-layout.png)
{:.dropshadow}

You can check how many rows and columns of the Forguncy page fit in the print size by clicking the [Dotted lines in print area] toggle button. The following figure shows the dotted line for the print area when [Margins] is set to "Normal", [Orientation] is set to "Landscape", and [Size] is set to "A5". You can confirm that the 21st row and up to the AF column fit as one page area.

![print-lines](/assets/images/product-images/print-lines.png)
{:.dropshadow}

By laying out the page so that it fits within this one-page print range, the layout will be one page for printing when exporting to PDF or Excel. By setting [Print Area], it is also possible to set a part of the page as the print area.

The basic concept of print size and extent is the same as above, except when you lay out elements whose area expands dynamically by displaying table data.

## Elements with dynamically added rows

In Excel/PDF export, there are the following two elements that dynamically add rows.

- list view
- repeater cell

These two elements set a fixed size area when the page is laid out, but when the page is displayed in a web browser, scrollbars are displayed depending on the amount of data to be displayed. Excel/PDF export will automatically add rows to output all data if scrollbars appear.

The following explanation assumes that the page is laid out as shown in the figure below.

In this case, the list view has an area tall enough to display up to 12 rows of data. This causes blank areas in the list view when less than 12 rows of data are displayed. In the figure below, the query condition is set so that only 7 items are displayed in the list view, so there is a blank area for 5 rows.

If you export this page to a PDF file, you can see that the layout in Forguncy Builder matches the layout in the exported PDF file.

From this state, check the Add blank lines in blank areas, apply styles, and formulas check option in the List View Settings dialog.

The display on the web browser does not change, but the result of the PDF export looks like the following figure.

You can see that styles such as borders and background colors have been applied to the blank areas.

Change the list view query conditions to display 17 data instead of 7. When the page is displayed in a web browser, scrollbars are displayed because it does not fit in the list view height of 12 lines.

If you export the page in this state to PDF, the result will be as shown in the following figure. You can see that 5 rows were dynamically added due to the 5 rows of data that did not fit in the list view height of 12 rows, and the layout spread over the second page.

For pages with list views or repeater type cells like this, rows are dynamically added vertically according to the number of data displayed there. As a result, the result will be different from the print area for one page laid out in Forguncy Builder. In order to repeat the layout of one page in Forguncy Builder for a page containing such dynamically added row elements, use the Report Repeat Settings feature.

## Report repeat settings

Report repetition setting is a function to set the area where the same layout will be made on all pages when rows are added dynamically in PDF export and a page break occurs.

For example, you can select the header area and footer area by using the report repeat setting, and it is possible to respond to layout changes due to page breaks.

This function is valid only for PDF export and does not affect the result of Excel export.

Select the entire row, which is an area for one page, and select Report Repeat Settings - Repeat Area Settings from the context menu.

With the row that will be the header area selected, select Report Repeat Settings - Header Area Settings from the context menu. The header area is a fixed layout that is printed at the top of all pages.

With the row that will be the footer area selected, select Report Repeat Settings - Footer Area Settings from the context menu. The footer area is a fixed layout that is printed at the bottom of every page.

Even if this setting is performed, the display on the web browser will not change, but the PDF export result will be as follows

You can confirm that the contents of the parts specified as the header area and footer area are output on the second page as well. However, while the height of the list view output on the 1st page is the same as the height of the list view when laid out with Forguncy Builder, the list view output on the 2nd page is as many as the output number It can be seen that the height of Therefore, the layout of the second page is different from the layout of the first page.

From this state, check the [Allocate list view area based on the number of rows at design time even after the second page] check option in the [List View Settings] dialog.

The result of the export to PDF looks like the image below. You can confirm that an area with the same height as the list view area on the first page is secured for the output of the second page, and blank lines are output in that area.

The height of the list view area on this second page is calculated based on the number of rows of the list view laid out by Forguncy Builder and the number of data to be output. In this case, 17 data were output for the height of the list view area that can display 12 rows. Therefore, on the second page, 5 cases, which is 17 cases minus 12 cases, will be displayed. On page 2, only 5 rows are output for 12 heights, so the number of missing height rows is 7 rows. This time, the list view template row height was set to 20 pixels, so 20 x 7 = 140 added a height of 140 pixels as the output area for the list view on page 2. Note that the missing height area is calculated based on the height of the template row. If the row defined as the list view does not have the same height including the template row, there will be a gap between the layout and the calculated missing height area, which is not the desired result. Hmm.

## Difference between Excel export and PDF export

Forguncy provides two commands, "Export to Excel (page)" and "Export to PDF" commands, both of which export the "page" originally created to be displayed on the screen to an Excel file or a PDF file. It's the same in that respect. However, even when exporting the same page, the output often looks different.

For example, create a Forguncy page like the one below and export it to Excel and PDF files.

The exported Excel file will look like this: You can see that the "Output" button and list view placed at the top are also exported to the Excel file sheet.

However, the result of exporting the PDF file is as shown in the following figure, and you can confirm that only the part where the repeater type cell was placed on the Forguncy page is output to the PDF file. The "Output" button and list view placed at the top will not be output.

This is because the [Print Area] function is used and only the repeater type cell area is set as the print area. For Excel export, this print area setting is reflected in the page settings of the Excel file. So if you view a print preview of the exported Excel file, you will see something like this:

You can see that it has almost the same layout as the output of the PDF export. However, unlike the PDF export, you can see that a page break has occurred in the middle of the repeater type cell template. This is because automatic control is performed so that a page break does not occur in the middle of one repeater type cell template only in the case of PDF export. Therefore, when using repeater type cells in Excel export, it is necessary to adjust the layout such as paper size, margins, and template size.

The main differences between Excel export and PDF export are:

- In PDF export, only the part specified in the print range is output, but in Excel export, the entire page is output, and the export print settings such as the print range are output as they are as Excel page settings.
- Repeater-type cells are controlled so that page breaks do not occur in the middle of the template only in PDF export.
- Report repeat settings only work for PDF exports.