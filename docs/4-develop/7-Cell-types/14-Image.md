---
layout: default
title: Image
parent: Cell Types
grand_parent: Develop
permalink: /develop/Cell-types/Image/
nav_order: 14
---

# {{ page.title }}

Create an area to display an image by using this cell type.

![image_celltype](/assets/images/product-images/image_celltype.png)
{:.dropshadow}

Note: If you want to insert an image as a page decoration without data binding, you can do so (regardless of the cell position or range) by selecting **Insert** → **Image**.
{:.note}

Steps to create a Image cell type:

- Select cells, merge, and go to the **Cell Type** drop-down list. 
- Select **Image** cell type. 
- Go to the **Cell Type** tab at the bottom of the right pane for the configuration.
You can do the following settings from here:

![image_celltype_settings](/assets/images/product-images/image_celltype_settings.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|Select Image|Selects an image file to display. <br/> ![image_upload_celltype_settings_default_image](/assets/images/product-images/image_upload_celltype_settings_default_image.png) <br/> Click **Import..** to import, or Click **Remove** to remove image file, or go to **Built-in Image** to select from built-in image icons.|
|Commands..|Sets the command to be executed when the image is clicked.|
|Set UI Permissions..|Show/hide and enable/disable the cell type for respective role. <br/> Note: This control has limitations in the list view.|
|Text|Sets the text that appears above the image.|
|Size Mode|Sets how the image is displayed on the webpage. <br/>-Original: Display at original size. <br/>-Fills: Fills the selected area while maintaining the aspect ratio of the image. <br/>-Contains: Display image to fit in the selected area.|
|Horizontal alignment|Sets the horizontal alignment of the image within the selected cell area: Left/Center/Right.|
|Vertical alignment|Sets the vertical alignment of the image within the selected cell area: Top/Center/Bottom.|
|Tooltip|Show the tooltip content when the mouse hovers over the image. <br/.> You can specify strings or cells here. Strings and cells can also be displayed by concatenating them with "&". <br/> Example: "This is an image." (Cell setting example) ”=A2” <br/> Note: This control has limitations in the list view.|
|Disabled|Disables user interaction with the image and renders it unusable. <br/> Note: This control has limitations in the list view.|
|Hidden|Make the page invisible. <br/> Note: This control has limitations in the list view.|

- Data concatenation is performed as necessary.