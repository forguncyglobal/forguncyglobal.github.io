---
layout: default
title: Record Navigation
parent: Cell Types
grand_parent: Develop
permalink: /develop/Cell-types/Record-navigation/
nav_order: 18
---

# {{ page.title }}

Record navigation allows you to switch between list view Records.

Example: Clicking an employee name in the employee directory will redirect to the individual page. By using Record navigation cell type, you can switch to other employee's information without returning to the employee directory screen.

![record_navigation_celltype_output1](/assets/images/product-images/record_navigation_celltype_output1.png)
{:.dropshadow}
![record_navigation_celltype_output2](/assets/images/product-images/record_navigation_celltype_output2.png)
{:.dropshadow}

Note: Record navigation cannot be set in the row template area of ​​a list view.
{:.note}

Steps to create a Record Navigation cell type:

![record_navigation_celltype](/assets/images/product-images/record_navigation_celltype.png)
{:.dropshadow}

- Select cells, merge, and go to the **Cell Type** drop-down list. 
- Select **Record Navigation** cell type. 
- The selected cells become the record navigation type.
- Go to the **Cell Type** tab at the bottom of the right pane for the configuration.

You can do the following settings from here:

![record_navigation_celltype_settings](/assets/images/product-images/record_navigation_celltype_settings.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|Data Table|Sets the data table to operate with record navigation.|
|Show record count|If unchecked, the record navigation will not display the record count between the buttons|
|**First Image** <br/>**Previous Image**  <br/>**Next Image**  <br/>**Last Image**|Sets the image used for record navigation. <br/>Click Change to select the image file to display. <br/> Click Import from Local File to import and select an image file, or click **Built-in Images** to select from built-in images. <br/> ![page_navigation_celltype_select_image](/assets/images/product-images/page_navigation_celltype_select_image.png)|
|Image size|Sets the size of the record navigation images (in pixels).|
|Spacing|Sets the record navigation button spacing (in pixels).|

Note: In case of multiple list views on the page when you set the transition target table to **Auto**, it may get associated with an unintended table. In this case, be sure to specify the transition target table.
{:.note}