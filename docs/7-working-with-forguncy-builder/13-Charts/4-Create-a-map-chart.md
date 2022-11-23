---
layout: default
title: Create a Map chart
parent: Charts
grand_parent: Working with Forguncy Builder
permalink: /develop/Charts/create-a-map-chart/
nav_order: 4
---

# {{ page.title }}

Use map charts to visualize geographical data, such as countries, regions, or cities. Forguncy's map chart differs from Excel's map chart in its specifications and functions.

In this example, we will use data from a table like the one in the figure below to visualize estimated population data for Miyagi Prefecture in a map chart.

Therefore, create a list view as shown in the figure below as the data source for the map chart.

## GeoJSON file
GeoJSON is a file format that expresses spatial data and coordinates using the JSON (JavaScript Object Notation) format, and is standardized as RFC 7946 (Internet Standard). For example, files in formats used by other prominent services and products, such as those supported by the Google Maps API.

Forguncy's map graph uses two files, an area GeoJSON file for representing countries and regions, and a point GeoJSON file for representing addresses and coordinates.

### area Geo JSON file
An area GeoJSON file is a GeoJSON file with data of "Polygon" or "MultiPolygon" as the geometry type. You should have polygon data in your geometry and name as a property, like in the image below.

Area GeoJSON files must be named "***_area.json" (where *** is any string) when used in Forguncy map graphs. "Fill Map" uses only this area GeoJSON file.

### point Geo JSON file
A point GeoJSON file is a GeoJSON file with data of "Point" as the geometry type. You should have the point data of your geometry and name as a property, like in the image below. This name value must match the name value in the area GeoJSON file.

The file name of the point GeoJSON file must be "***_point.json" (where the *** part is any string) when used in Forguncy map graphs. "Bubble Map" and "Heat Map" use this point GeoJSON file in addition to the area GeoJSON file.

## colored map
- With the list view selected, expand the Map button dropdown on the Insert tab of the ribbon and click Filled Map.
- In the GeoJSON Settings dialog, click the Open folder for placing GeoJSON files... hyperlink.
- Copy the prepared area GeoJSON file and point GeoJSON file to the folder called "UserMapFile" on the opened explorer. Here, copy the files named "Miyagi_area.json" and "Miyagi_point.json". In addition, only the area GeoJSON file is used in the "paint map", but the point GeoJSON file is also copied in order to create the "bubble map" and "heat map".

Reference: This "UserMapFile" is a folder that can be used for each Forgunncy project (FGCP file). To make the GeoJSON file commonly referenced in all Forguncy projects opened on that computer, place the GeoJSON file in the following folder: "Forguncy\Website\DesignerResources\Map" folder under the folder where Forguncy Builder is installed.

- Back in the GeoJSON Settings dialog, click the icon (Get Latest GeoJSON File List) in the upper right corner.
- Select "Miyagi Prefecture" from the drop-down list for [area GeoJSON file], and click the [OK] button to close the dialog. As shown in the following figure, the "Painted Map" graph will be inserted, so adjust the position, size, style, etc. as desired.
- Click the Start (Debug) button from the Home tab on the ribbon to see how it works. You can see that the municipalities on the map are colored according to the estimated population values.

## bubble map
I will explain the procedure from the state where the creation of the above "painting map" is completed.

- Select the chart and click the Change Chart Type button from the Design tab in the Chart Tools contextual tab of the ribbon.
- Select [Bubble Map] in the [Change Graph] dialog and click the [OK] button.
- Click the Configure GeoJSON button from the Design tab in the Graph Tools contextual tab of the ribbon.
- In the [GeoJSON Settings] dialog, select "Miyagi Prefecture" from the drop-down list for [point GeoJSON file], and click the [OK] button to close the dialog.
- Click the Start (Debug) button from the Home tab on the ribbon to see how it works. It can be confirmed that bubbles of a size corresponding to the estimated population value are displayed at the location of each city/town/village office on the map.

## heat map
I will explain the procedure from the state where the creation of the above "bubble map" is completed.
- Select the chart and click the Change Chart Type button from the Design tab in the Chart Tools contextual tab of the ribbon.
- Select [Heatmap] in the [Change Graph] dialog and click the [OK] button.
- Click the Start (Debug) button from the Home tab on the ribbon to see how it works. You can see that the circles with gradations of sizes corresponding to the estimated population values ​​are displayed at the positions of each city/town/village office on the map.

## Usage Guide
Legends have different settings than map charts in Excel. The map chart legend settings in Forguncy are listed below. Note that legends cannot be used with "bubble maps".