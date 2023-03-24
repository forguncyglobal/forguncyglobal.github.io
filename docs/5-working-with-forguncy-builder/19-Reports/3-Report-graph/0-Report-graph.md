---
layout: default
title: Report Graph
parent: Reports
grand_parent: Working with Forguncy Builder
permalink: /develop/reports/report-graph/
nav_order: 3
has_children: true
has_toc: true
---

# {{ page.title }}

Charts are useful for observing changes in data over time, comparing different groups or portions of data, and determining relationships between variables.

Steps to add chart in a report are:

- Create a report.
- Click or drag and drop **Chart** from the toolbox.

![report-add-chart](/assets/images/product-images/report-add-chart.png)
{:.dropshadow}

- You can change the template after adding the Chart component to the designer area. Simply select a Chart and switch by choosing **Chart** → **Set Plot Template**.

![report-switch-chart](/assets/images/product-images/report-switch-chart.png)
{:.dropshadow}

The following chart types are available:

|Chart Type|Description|
|:--|:--|
|**Vertical Bar**|Vertical Bar, Stacked Vertical Bar, Stacked Vertical Bar (%)|
|**Horizontal Bar**|horizontal bar, laminated horizontal bar, laminated horizontal bar (%)|
|**Polyline**|Polyline, smooth line|
|**Area**|Area, lamination area, lamination area (%)|
|**Yen**|circle, donut|
|**Spiral**|spiral, laminated spiral, laminated spiral (%)|
|**Polar**|Polar, Stacked Polar, Stacked Polar (%)|
|**Radar**|Radar Area, Radar Bubble, Radar Scatterplot, Radar Line|
|**Others**|Pyramid, Funnel, Bubble, Scatterplot, Gantt, Candlestick, HiLoOpenClose, HiLoClose|

- Concatenate the data into each region. Selecting the chart data region will reveal the settings such as data fields, category fields, and encoding. Drag and drop the appropriate fields from your dataset into these areas to bind them.

![report-charts-concatenate-data](/assets/images/product-images/report-charts-concatenate-data.png)
{:.dropshadow}

|**Data Field**|Set the field that will be the value.|
|**Categorical field**|Set the field that will be the data category.|
|**Advanced**|Sets which fields are subcategories of data values.|
|**Color (color legend)**|Sets the field used to display the legend.|
|**Text**|Sets the field to display as a data label or tooltip.|