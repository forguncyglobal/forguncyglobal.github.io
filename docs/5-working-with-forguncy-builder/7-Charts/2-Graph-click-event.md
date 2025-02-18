---
layout: default
title: Graph Click Event
parent: Charts
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Charts/graph-click-event/
nav_order: 2
---

# {{ page.title }}

When you click the graph, you can define a click event such as acquiring a value or executing a command according to the clicked position. This function can use the following graph types.

- Clustered Column, Stacked Column, 100% Stacked Column
- Line with Markers, Stacked Line with Markers, 100% Stacked Line with Markers
- Circle, Donut
- Clustered Bar, Stacked Bar, 100% Stacked Bar
- Scatter Plot, Scatter Plot (Smooth Line and Markers), Scatter Plot (Line and Markers)
- Bubble
- Paint map, Bubble map

Steps to set a click event are:

## Passing Values ​​(Property Setting)

- Select the chart object and click **Change Chart Commands** on the Design tab of the **Chart Tools** contextual tab on the ribbon.
- Set the series name, category, and value in the **Click Event** dialog, then click the OK button to close the dialog.
- Click the **Start** (Debug) button from the **Home** tab on the ribbon to see how it works. When you click the graph, the series, categories, and values ​​set according to the clicked position are displayed on the page.

## Command

- Create a page that opens as a popup window.
- Select the Chart and click **Click Event** on the **Design** tab of the **Chart Tools** contextual tab.
- Click the **Commands...** hyperlink in the **Click Events** dialog for setting commands.
- Set the **Show Popup Window** command, set the transition destination page and transition destination cell.
- Click the **Start** (Debug) button from the **Home** tab to see how it works. When you click the graph, the detailed data will be displayed in the list view on the pop-up window according to the clicked position.

