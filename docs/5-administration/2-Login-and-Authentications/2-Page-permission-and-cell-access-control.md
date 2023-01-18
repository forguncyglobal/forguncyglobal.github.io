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

|Roles|Description|
|:--|:--|
|**Everyone**|If checked, anyone can view the page regardless of whether they are logged in. No login screen is displayed. <br/>This setting will not be displayed if Windows authentication is selected). This setting takes precedence over other role settings.|
|**Authenticated Users**|By checking, only logged-in users can view the page. By default this is checked. <br/> If you have opted for forms authentication, a login screen will be displayed to determine the user. For Windows authentication, the authentication dialog may or may not be displayed depending on the type and settings of the web browser.|
|**Administrator**|Forguncy's default admin role. <br/> By checking, only users who belong to the Administrator role and have logged in can view the page. A login screen is displayed to determine the user.|
|**Other added roles**|By checking, only users who belong to the role and have logged in can view the page. A login screen is displayed to determine the user. The roles displayed here are the ones created in [User Service Manager](https://docs.forguncy.net/working-with-forguncy-builder/administration/user-service-manager/) in advance during development.|

You can filter searches for roles and pages as follows:

![authority-management-filter-searches](/assets/images/product-images/authority-management-filter-searches.png)
{:.dropshadow}

### Precautions when Republishing applications

If you republish your application after changing page view permission settings, you must check the Override page view permission and cell access control settings check option when republishing your application. If you republish the application without checking this check option, the changed page view permission settings will not be reflected in the published application.

### Changing Page View Permissions in Forguncy Server Admin Portal

After publishing the application, it is possible to change the page viewing permission setting on the Forguncy server management portal.





