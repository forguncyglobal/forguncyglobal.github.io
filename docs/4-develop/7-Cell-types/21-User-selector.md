---
layout: default
title: User Selector
parent: Cell Types
grand_parent: Develop
permalink: /develop/Cell-types/User-selector/
nav_order: 21
---

# {{ page.title }}

User Selector cell type is a combo box that allows user to select user from the dropdown list of registered useres in Forguncy.

![user_selector_celltype](/assets/images/product-images/user_selector_celltype.png)
{:.dropshadow}

![user_selector_celltype_output](/assets/images/product-images/user_selector_celltype_output.png)
{:.dropshadow}

Note: For user registration, please refer to [User Management](https://docs.forguncy.net/user-services/#user-services).
{:.note}

Steps to create a Image Uploader cell type:

- Select cells, merge, and go to the **Cell Type** drop-down list. 
- Select **User Selector** cell type. 
- The selected cell becomes a User selector combo box.
- Adjust the cell width so that the user name can be seen when the list is dropped down.
- Go to the **Cell Type** tab at the bottom of the right pane to configure the user selection combo box.
You can do the following settings from here:

![user_selector_celltype_settings](/assets/images/product-images/user_selector_celltype_settings.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|Commands..|Sets the command to run when the value changes. <br/> Note: This control has limitations in the list view.|
|Set UI Permissions..|Show/hide and enable/disable the cell type for respective role. <br/> Note: This control has limitations in the list view.|
|Default Value|Specifies the default selection. You can also use formulas.|
|Limit Users to Following Role|Specify a role to display users having that role only. If no role is specified, all users registered in Forguncy Server will be displayed.|
|Display Column|Select the fields to be displayed. <br/>This field is not visible or configurable on mobile pages.|
|User details to show in the list|Multiple items such as *Username*, *Full name*, and *Email address* can be selected to display in the drop-down list. <br/>This field is not visible or configurable on mobile pages.|
|Auto Filter|A feature that only displays items that match the value entered by the user. Specify either start match or partial match.|
|Watermark|Specify the watermark character to be displayed when there is no selection. <br/>This field is not visible or configurable on mobile pages.|
|Miscellaneous|-Read-only:When checked, you can only view the drop-down list and cannot make a selection. <br/> -Selection only: When checked, it does not accept input by the user, only selection from the drop-down list is possible. This item is not visible and cannot be set on mobile pages (only input by selection is supported). <br/>-Select text content on focus:All values ​​are automatically selected when the focus is acquired. <br/> Note: This control has limitations in the list view.|

- Data concatenation is performed as necessary.