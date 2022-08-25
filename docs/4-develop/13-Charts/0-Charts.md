---
layout: default
title: Charts
parent: Develop
permalink: /develop/Charts/
nav_order: 13
has_children: true
has_toc: true
---

# {{ page.title }}

You can create a graph in the same way as you create charts in the Excel by using the chart function. 

## Chart Type
Forguncy supports the following chart types. If you want to create a combo chart instead of a single chart, see [Create a Combo Chart](http://localhost:4000/develop/Charts/create-a-combo-chart/#create-a-combo-chart).

- Column Chart
- Line Graph
- Pie Chart
- Horizontal Bar Chart
- Area Chart
- Radar Chart
- Scatter Plot
- Bubble
- Map

![chart-types](/assets/images/product-images/chart-types.gif)
{:.dropshadow}

## Chart Data Source

### Cell Range

- Select a cell range as the data source and go to **Insert** ribbon tab. 
- Select the required chart type. 
- The data selection method will be the same as in Excel.
- Right-click on the chart and select **Select data**.

![insert-chart](/assets/images/product-images/insert-chart.png)
{:.dropshadow}

**Select Data Source** dialog will appear.

![select-data-source](/assets/images/product-images/select-data-source.png)
{:.dropshadow}

Click **Edit** to edit series.  Specify the cell range  as required.   

![chart-edit-series](/assets/images/product-images/chart-edit-series.png)
{:.dropshadow}

### List View

- Select the entire list view and go to **Insert** ribbon tab. 
- Select the required chart type.
- The data source is *List View*.

The design-time preview may take a long time, depending on the data source specified in the list view. You can disable the preview display by disabling the Show preview, see application settings.

In list view data source, the selection of series and horizontal axis items is slightly different than cell range. The series value specifies a single cell like *=C13* which means that the data of the field linked to the C13 cell will be selected as the series. Also, you cannot specify a cell range (multiple items) for the items on the horizontal axis.

### Pivot Table

If you click a chart type for a pivot table type cell, the data source will be *List View*. 

Scatter, bubble, and map chart types are not available when using a PivotTable as a data source.

Also, you cannot edit legend items or horizontal axis labels in the **Select Data Source** dialog. It is necessary to change the settings on the pivot table side based on the graph you want to display.

## How to create a graph

Insert a chart by doing the following:

- Specify the data to be graphed in cell range, list view, or PivotTable. 
- Go to **Insert** ribbon tab.
- Select the required chart type. 
- Go to **Design**, **Layout**, and **Format** tabs in **Chart Tools** to change the format of the chart, or right-click the chart and choose relevant option.

Note: The Scatter, Bubble, and Map charts are not available when using a PivotTable as a data source. If the data source is a list view, the **Switch Row/Column** button cannot switch the series and horizontal axis items. When the data source is list view, only single cell of the row can be selected as items on the horizontal axis, and only data that expands vertically can be represented as a graph.
{:.note}


