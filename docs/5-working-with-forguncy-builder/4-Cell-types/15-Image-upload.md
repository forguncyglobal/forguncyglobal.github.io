---
layout: default
title: Image Upload
parent: Cell Types
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Cell-types/Image-Upload/
nav_order: 15
---

# {{ page.title }}

This cell type creates an image upload area in the selected cells. Clicking on this opens an image file selection dialog. It allows user to choose and upload desired image. After uploading, the image will be displayed in the area.

![image_upload_celltype](/assets/images/product-images/image_upload_celltype.png)
{:.dropshadow}

![image_upload_celltype_output](/assets/images/product-images/image_upload_celltype_output.png)
{:.dropshadow}

You can also upload image files by dragging and dropping them into the image upload area (except when created in the row template part of the list view). 
You can replace image with another after uploading by simply clicking on the image uploader area and choose another image.

Note: Even if you drag and drop multiple files, only one file will be uploaded.
{:.note}

Use the Delete key of your keyboard to delete the uploaded image when created in the row template portion of the ListView.

Steps to create a Image Uploader cell type:

- Select cells, merge, and go to the **Cell Type** drop-down list. 
- Select **Image Upload** cell type. 
- The selected cell becomes an image uploader.
- Go to the **Cell Type** tab at the bottom of the right pane for the configuration.
You can do the following settings from here:

![image_upload_celltype_settings](/assets/images/product-images/image_upload_celltype_settings.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|Choose Default Image: Select Image|Allows to set a default image to display when no image has been uploaded. <br/> ![image_upload_celltype_settings_default_image](/assets/images/product-images/image_upload_celltype_settings_default_image.png) <br/> Click **Import..** to import, or Click **Remove** to remove image file, or go to **Built-in Image** to select from built-in image icons.|
|Set UI Permissions|Show/hide and enable/disable the cell type for respective role. <br/> Note: This control has limitations in the list view.|
|Size Mode|Sets how the image is displayed on the webpage. <br/>-Original: Display at original size. <br/>-Fills: Fills the selected area while maintaining the aspect ratio of the image. <br/>-Contains: Display image to fit in the selected area.|
|Horizontal alignment|Sets the horizontal alignment of the image within the selected cell area: Left/Center/Right.|
|Vertical alignment|Sets the vertical alignment of the image within the selected cell area: Top/Center/Bottom.|
|Read-only|It makes the cell type as read only and user will not be able to upload images.|
|Configure Image Upload|Opens **Configure Image Upload** dialog to select whether to automatically reduce the image. When automatic reduction is enabled, if the image that the user tries to upload exceeds the maximum width or height specified, it will be compressed and upload it. <br/> Forguncy creates and save the following three types of sizes on the Forguncy Server side based on the uploaded image. <br/>-Original size <br/>-400px (not created if the uploaded image is less than 400px) <br/>-150px (will not be created if the uploaded image is less than 400px) <br/>-When the uploaded image is displayed, the optimal image is sent from Forguncy Server to the client according to the size of the display area.|

- Data concatenation is performed as necessary. 

![image_upload_celltype_data_storage](/assets/images/product-images/image_upload_celltype_data_storage.png)
{:.dropshadow}

When storing image data in Forguncy's internal database using image upload type cells, the value stored in the database table as the image filename, not the image data. The data type of the field used is image type.