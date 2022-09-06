---
layout: default
title: Conditional Formatting of Charts
parent: Charts
grand_parent: Develop
permalink: /develop/Charts/conditional-formating-of-charts/
nav_order: 3
---

# {{ page.title }}

Forguncy charts can change dynamically depending on the data in the database, so you can't specify the style individually like Excel. Conditional formatting can be used to style the chart elements. 

Note: This function cannot be used if the data source of the graph is a pivot table type cell.
{:.note}

Whether or not conditional formatting can be used and the items that can be set differ depending on the chart type. Conditional formatting is not available for charts other than the chart types listed in Chart Types in the following table.

|Chart Type|Category|Value|Percent <br/> value (decimal)|X-axis value, <br/> Y-axis value|Upper,<br/> lower|Bubble <br/> Size|Background <br/> Color|line <br/> Style|Marker <br/> Options|
|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--|
|Clustered Column, Stacked Column, Clustered Horizontal Bar, Stacked Horizontal Bar|○|○|-|-|○|-|○|○|-|
|100% Vertical Stacked Bar, 100% Horizontal Stacked Bar|○|○|○|-|○|-|○|○|-|
|100% Stacked line with markers|○|○|○|-|○|-|○|-|○|
|Circle, donut|○|○|-|-|○|-|○|○|-|
|Line with Markers, Stacked Line with Markers|○|○|-|-|○|-|○|-|○|
|Scatter Plot, Scatter Plot (Smooth Line and Markers), Scatter Plot (Line and Markers)|-|-|-|○|○|-|○|-|○|
|Bubble|-|-|-|-|○|○|○|-|-|
|Bubble Map|○|○|-|-|○|-|○|-|-|

Here is an example of setting conditional formatting for the chart below.

![conditional-formating-chart](/assets/images/product-images/conditional-formating-chart.png)
{:.dropshadow}

Conditional formatting can set rules based on category, value, ranking (top and last). 

Note:The first rule has the highest priority, and the priority decreases from the top to bottom.
{:.note}

![chart-conditional-formating](/assets/images/product-images/chart-conditional-formatting.png)
{:.dropshadow}

- Select the chart object and click **Conditional Formatting** on the **Design** tab of the **Chart Tools** contextual tab on the ribbon.
- Create a new rule in the **Chart Conditional Formatting** dialog, configure it as shown in the figure and click **OK**.

### Category

![conditional-formating-chart-category](/assets/images/product-images/conditional-formating-chart-category.png)
{:.dropshadow}

### Value

![conditional-formating-chart-values](/assets/images/product-images/conditional-formating-chart-values.png)
{:.dropshadow}

### Ranking (Top and Last)

![conditional-formating-chart-ranking](/assets/images/product-images/conditional-formating-chart-ranking.png)
{:.dropshadow}

### Percent value (Decimal)
Available for 100% Stacked Column, 100% Stacked Horizontal Bar, and 100% Stacked Line with Markers chart types. 

![conditional-formating-chart-percentage](/assets/images/product-images/conditional-formating-chart-percentage.png)
{:.dropshadow}


<!--
<head>
    <style>
        table,
        th,
        td {
            border: 0.5px solid black;
            border-collapse: collapse;
            padding: 0.5px;
            text-align: center;
        }
        table{
           widht:5px;
        }
    </style>
</head>

<body>
    <center>
        <table>
            <tr>
                <th>Chart Type</th>
                <th colspan="6">Conditions</th>
                <th colspan="3">Styling</th>
            </tr>
            <tr>
                <td> </td>
                <td>Category</td>
                <td>Value</td>
                <td>Percent value (decimal)</td>
                <td>X-axis value, Y-axis value</td>
                <td>Upper, lower</td>
                <td>Bubble size</td>
                <td>Background color</td>
                <td>Line style</td>
                <td>Marker options</td>
            </tr>
            

        </table>
    </center>
</body>

-->











