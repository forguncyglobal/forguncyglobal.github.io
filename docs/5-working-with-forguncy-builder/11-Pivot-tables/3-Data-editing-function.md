---
layout: default
title: Data Editing Function
parent: Pivot Tables
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Pivot-tables/data-editing-function/
nav_order: 3
---

# {{ page.title }}

A PivotTable provides the ability for users to add, edit, and delete data on the PivotTable. This feature is only available for pivot tables that meet the following specific conditions:

- The list view used as the data source is set to be editable.
- Aggregation type of the **Values** field is *First*.

Note: Allowing editing in the Pivot Table automatically sets the aggregation type to *First*.
{:.note}

The data editing function can be used only when aggregation or calculation is not performed on the pivot table. So, you can use this functionality when you want to lay out monthly data in a horizontal direction (that cannot be expressed in the list view) and edit it.

This function only supports single cell editing. It is not possible to batch edit multiple cells using copy and paste.

- Make list view (the one being used as data source for the pivot table) editable.
- Select pivot table and open **Pivot Table Settings**.
- Enable editable option. The aggregation method will automatically changed to *First*.
- Open the **Field Settings** dialog of the value field.
- In the **Total Summarized** tab, disable *Keep same Aggregation with Value* Field Aggregation check option. Instead, select Aggregation Type as *Sum*.
- Click **OK** to close the dialog.