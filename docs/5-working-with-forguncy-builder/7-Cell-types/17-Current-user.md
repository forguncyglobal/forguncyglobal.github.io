---
layout: default
title: Current User
parent: Cell Types
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Cell-types/current-user/
nav_order: 17
---

# {{ page.title }}

You can display the logged-in username by using **Current User** cell type.

Note: This cell type cannot be set in the row template area of ​​a listview.
{:.note}

![currentuser_celltype](/assets/images/product-images/currentuser_celltype.png)
{:.dropshadow}
This screenshot is showing the user icon, current username, and three outstanding [workflow](https://docs.forguncy.net/develop/Workflows/) notifications that are assigned to this user.

By clicking **▼** you can **Edit profile**, **Change password**, and **Logout**. It is displayed for apps whose authentication mode is "form authentication". You can only **Logout** when using the **Authentication Provider for SAML 2.0**.

Steps to create Current User cell type:

- Select a cell and go to the **Cell Type** drop-down list. 
- Select **Current User** cell type. The selected cell becomes the Current user type.
- Click the **Cell Type** tab at the bottom of the right pane to configure login user settings.

![currentuser_celltype_settings](/assets/images/product-images/currentuser_celltype_settings.png)
{:.dropshadow}

|Control|Description|
|:--| :--|
|**Show user display name**|Display *Username* and if unchecked, then the user's *Full Name* will be displayed.|
|**Show user picture**|Display user icons|
|**Show dropdown**|Displays **▼** for a drop-down list that allows user to select *Edit Profile*, *Change Password*, and *Logout*. <br/> ![currentuser_celltype_output](/assets/images/product-images/currentuser_celltype_output.png)|
|**Show notification badge**|Displays the number of workflow notifications assigned to the logged-in user, if any.|
|**Navigate for notification**|If there are workflow notifications, clicking on the number of notifications will redirect the user to the specified page.|
|**Navigation on signout..**|Allows navigation settings on signout. It has four options: <br/>- Stay on Current page (no transition) <br/>- Go to the Homepage <br/>- Go to specific page. For this you need to select the page for transition. <br/>- Go to specefic URL. For this enter the URL starting with *http://* or *https://*. <br/> <br/> Note: The default is **Homepage**.|

- Data concatenation is performed as necessary.

Note: The Current User cell type cannot display the data of a data-bound table. However, user information such as the currently logged in user account name can be registered/updated in the data-linked table.
{:.note}

