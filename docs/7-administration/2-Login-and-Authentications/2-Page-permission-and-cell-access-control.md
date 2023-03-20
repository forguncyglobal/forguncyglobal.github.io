---
layout: default
title: Page Permission and Cell Access Control
parent: Login and Authentications
grand_parent: Administration
permalink: /administration/login-and-authentications/page-permission-and-cell-access-control/
nav_order: 2
---

# {{ page.title }}

## Page Permission

You can limit the use of applications by setting viewing permissions for each page for logged-in users and roles.

Use this permission setting if you want only specific users to be able to operate the page. 
n the case of data-level access control, it is possible to restrict not only database access from the screen but also access from the API.

This section describes how to set permissions for pages.

![authority-management](/assets/images/product-images/authority-management.png)
{:.dropshadow}

- Go to **Security** tab.
- Clicking the **Authority Management** option will open the **Authority Manager Window**.
- Set pages for respective roles. 

Note: When setting permissions for each role, it is necessary to log in to the [User Service Manager](https://docs.forguncy.net/working-with-forguncy-builder/administration/user-service-manager/), add roles in advance.
{:.note}

### List of Roles with Privileges

|Roles|Description|
|:--|:--|
|**Everyone**|If checked, anyone can view the page regardless of whether they are logged in. No login screen is displayed. <br/>This setting will not be displayed if Windows authentication is selected). This setting takes precedence over other role settings.|
|**Authenticated Users**|By checking, only logged-in users can view the page. By default this is checked. <br/> If you have opted for forms authentication, a login screen will be displayed to determine the user. For Windows authentication, the authentication dialog may or may not be displayed depending on the type and settings of the web browser.|
|**Administrator**|Forguncy's default admin role. <br/> By checking, only users who belong to the Administrator role and have logged in can view the page. A login screen is displayed to determine the user.|
|**Other added roles**|By checking, only users who belong to the role and have logged in can view the page. A login screen is displayed to determine the user. The roles displayed here are the ones created in [User Service Manager](https://docs.forguncy.net/working-with-forguncy-builder/administration/user-service-manager/) in advance during development.|

You can filter searches for roles and pages as follows:

![authority-management-filter-searches](/assets/images/product-images/authority-management-filter-searches.png)
{:.dropshadow}

## Cell Access Control

For a specific cell type, you can set whether it can be used, displayed, hidden, or whether it can be edited depending on the role of the login user.

Note: This permission setting is only for access control on the screen. When access control is applied to a text box cell type that can update a field in the database, it is not possible to update from the screen, but it is possible to update from other means such as API. If you want access control over such operations , consider using data-level access control.
{:.note}

<!-- Also, if you use this function to disable or hide a cell, you cannot use the *[Set Cell Properties]* command to cancel that state. -->

Cell access control is available for the following cell types. In addition, this function cannot be used in the cell type placed in the list view cell template.

|Cell Type|Enabled authority|View permission|Edit permission|
|:--|:--|:--|:--|
|Button|✓|✓|-|
|Hyperlink|✓|✓|-|
|Image|✓|✓|-|
|Text Box|✓|✓|✓|
|Multiline Text Box|✓|✓|✓|
|Combo Box|✓|✓|✓|
|Date|✓|✓|✓|
|Time|✓|✓|✓|
|Numerical Value|✓|✓|✓|
|Check Box|✓|✓|✓|
|Check Box Group|✓|✓|✓|
|Radio Group|✓|✓|✓|
|User Selection combo Box|✓|✓|✓|
|Image Upload|✓|✓|✓|
|Attachment|✓|✓|✓|
|Menu|-|✓|-|

Steps to set cell access control are as follows-

![cell-access-control-set-UI-permission](/assets/images/product-images/cell-access-control-set-UI-permission.png)
{:.dropshadow}

- Select the target cell type and go to **Cell Type** tab of the right pane.
- Click **Set UI Permissions..**.
- In the **UI Permission Settings** dialoge 
    - Check the *Enable* check box on the **Enable Permission** tab and select any role to make the target cell available only to members belonging to a specific role.

    ![cell-access-control-set-enable-permission](/assets/images/product-images/cell-access-control-set-enable-permission.png)
    {:.dropshadow}

    - Check the *Enable* check box on the **Visible Permission** tab and select any role to make the target cell visible only to members belonging to a specific role.

    ![cell-access-control-set-visible-permission](/assets/images/product-images/cell-access-control-set-visible-permission.png)
    {:.dropshadow}

    - Check the *Enable* check box on the **Editable Permission** tab and select any role to make the target cell editable only to members belonging to a specific role.

    ![cell-access-control-set-editable-permission](/assets/images/product-images/cell-access-control-set-editable-permission.png)
    {:.dropshadow}

- Click the **Start** button on the **Home** ribbon tab to debug and see your application in action.

Read here to know about [privileges for respective roles](#list-of-roles-with-privileges).

## Precautions when Republishing applications

If you republish your application after changing page view permission/ new cell access control settings, you must check the Override page view/display permission and cell access control settings check option when republishing your application. If you republish the application without checking this check option, the changed/new settings will not be reflected in the published application.

## Changing Page View Permissions and Access Control in Forguncy Server Admin Portal

After publishing the application, it is possible to change the page viewing permission and cell's access control settings on the Forguncy server management portal.



