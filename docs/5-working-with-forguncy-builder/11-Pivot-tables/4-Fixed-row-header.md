---
layout: default
title: Fixed Row Header
parent: Pivot Tables
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Pivot-tables/fixed-row-header/
nav_order: 4
---

# {{ page.title }}

## Fixed Row Header

If the pivot table has a large number of columns, scrolling horizontaly  may cause the row headers to disappear.

By setting the row header fixed function, you can always display the row header even when scrolling horizontally.

- Select Pivot and open **Pivot Table Settings** available on the right pane.
- Go to **Other** tab.
- Select the field you want to freeze from the **Frozen Field** drop-down list. The default value is *Freeze all fields*.

All fields displayed as row headers are displayed in a drop-down list.

If "Freeze All Fields" is set, all row headers will be fixed.
If "Unfixed" is set, all row headers will not be fixed. When scrolling horizontally, the row headers are also scrolled.

Note: The default value for [Fixed Fields] is "Fix All Fields".
{:.note}

### Fixed Column Border Color

The default border color for fixed columns is No Fill. This setting value can be changed in [Cell style] of the pivot table.

After selecting the PivotTable type cell, right-click and edit the set style from [Home] ribbon tab - [Cell Style].
In the Cell Style Settings dialog, confirm that Entire Table is selected for Node, and set the Fixed Column Border Color.
