---
layout: default
title: Page Navigation
parent: Cell Types
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Cell-types/Page-navigation/
nav_order: 19
---

# {{ page.title }}

Page navigation allows you to switch between list view pages.

![page_navigation_celltype_with%20listview](/assets/images/product-images/page_navigation_celltype_with%20listview.png)
{:.dropshadow}

Note: Page navigation cannot be set in the row template area of ​​a list view. Also, it is not available for ODBC data sources. Also, it cannot be used when using summary fields.
{:.note}

Steps to create a Page Navigation cell type:

![page_navigation_celltype](/assets/images/product-images/page_navigation_celltype.png)
{:.dropshadow}

- Select cells, merge, and go to the **Cell Type** drop-down list. 
- Select **Page Navigation** cell type. 
- The selected cells become the page navigation type.
- Go to the **Cell Type** tab at the bottom of the right pane for the configuration.

You can do the following settings from here:

![page_navigation_celltype_settings](/assets/images/product-images/page_navigation_celltype_settings.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|Pageing Listview Name|Sets the list view to operate with page navigation.|
|Row Count in Every Page|Allows you to enter the number of rows to display per page.|
|**First page** image <br/>**Previous page** image <br/>**Next page** image <br/>**Last page** image|Sets the image used for page navigation. <br/>Allows you to select an image to display. <br/>Click Import from Local File to import and select an image file, or click Built-in Images to select from built-in images. <br/> ![page_navigation_celltype_select_image](/assets/images/product-images/page_navigation_celltype_select_image.png)|
|image size|Sets the size of the page navigation images (in pixels).|
|Spacing between each button|Sets the page navigation button spacing (in pixels).|

Note: Page navigation does not support adding/deleting records within the list view. If you want to add or delete records, use the **Update Table Data** command or use the "Delete records" command in the list view.
{:.note}

