---
layout: default
title: Export Pivot Table
parent: Pivot Tables
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Pivot-tables/export-pivot-table/
nav_order: 5
---

# {{ page.title }}

It is possible to export pivot table type cells to Excel and PDF, but the list view specified as data source of the pivot table must meet the following conditions:

- The Column Header checkbox should be checked and number of Column Header Rows is set to 1.
- Column header cells are not merged.
- No blank cells on the column headers.
- The selected column check box is not checked.
- The *Summary row* check box is not checked.

Note: Graphs having Pivot Table as data source will not be exported.
{:.note}

To increase the export speed, turn off *Maintain the order in the data source when exporting* flag available in *Other* tab of *Pivot Table Settings*. However, the order will not be the same as on the screen, but will be similar to the default order of Excel.

