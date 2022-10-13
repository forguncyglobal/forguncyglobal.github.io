---
layout: default
title: Attachment
parent: Cell Types
grand_parent: Develop
permalink: /develop/Cell-types/Attachment-upload-box/
nav_order: 16
---

# {{ page.title }}

Create an area for uploading attachments in a cell type. Clicking on the *Add* button will open a dialog. This will allow you to select a file. The file name will be displayed in the area. You can delete the added file by clicking the *Delete* button.

![attachment_celltype](/assets/images/product-images/attachment_celltype.png)
{:.dropshadow}

You can also select multiple files by holding down the *Ctrl key* when selecting files. You can also upload multiple files by dragging and dropping them into the Attachments area (unless you created them in the row template portion of the ListView).

Note: If you create it in the row template part of the list view, it will be displayed differently. 
{:.note}

<!-- Click the button on the right side of the cell to display the file selection dialog. The *Delete* link shown in the image above will not be displayed. Use the Delete key on your keyboard to delete the uploaded file. -->

Steps to create a Attachment cell type:

- Select cell and go to the **Cell Type** drop-down list. 
- Select **Attachment** cell type. 
- The selected cell becomes a Attachment type.
- Go to the **Cell Type** tab at the bottom of the right pane to configure the settings for the attachment box.

You can do the following settings from here:

![attachment_celltype_settings](/assets/images/product-images/attachment_celltype_settings.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|Set UI Permissions|Show/hide and enable/disable the cell type for respective role. <br/> Note: This control has limitations in the list view.|
|Read-only|It makes the cell type as read only and user will not be able to upload attachments.|
|Configure File Upload Restrictions|Set the extension of files that can be uploaded, the file size, and the limit on the number of files that can be uploaded at once. ![attachment_celltype_configure_file_upload_restrictions](/assets/images/product-images/attachment_celltype_configure_file_upload_restrictions.png) <br/>-To specify multiple extensions, separate them with commas. If you don't want to limit the file extensions that can be uploaded, check the **No Limitations** check option. <br/>-To specify the upload file size limit, uncheck **No Limitations** and enter the maximum size (MB). <br/>-To specify a limit on the number of files that can be uploaded at one time, uncheck **No Limitations** and enter the maximum number of files.|

- Data concatenation is performed as necessary. 

When storing attachments in Forguncy's internal database using attachment type cells, the value stored in the database table is the file name of the attachment, not the attachment itself. 

The data type of the field required for data binding with this cell type is the attachment type. <br/> In the development environment (Forguncy Builder), images are saved in the following path.
*C:\ProgramData\Forguncy\UserName\<arbitrary number>\WebSite\Upload*
