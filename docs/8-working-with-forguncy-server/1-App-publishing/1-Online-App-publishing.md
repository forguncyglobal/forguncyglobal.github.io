---
layout: default
title: Online App Publishing
grand_parent: Working with Forguncy Server
parent: App Publishing
permalink: /working-with-forguncy-server/app-publishing/online-app-publishing/
nav_order: 2
has_children: false
has_toc: false
---

# {{ page.title }}

Published applications are stored by default in the following folder on the computer where Forguncy Server is installed:

- *C:\Users\Public\Documents\ForguncyServer* in Windows 
- */opt/ForguncySites/ForguncyServer/* in Linux

The storage location can be changed from the **Save Folder** setting of the server management portal. 

The steps for app publishing using Forguncy Server are as follows-

- Go to **Publish** tab in Forguncy Builder and click **Server**.

![app-publishing](/assets/images/product-images/app-publishing.png)
{:.dropshadow}

- Set the required information in the **Publish Settings** dialog.

![app-publishing-settings-dialog](/assets/images/product-images/app-publishing-settings-dialog.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|**Server**|Specify the computer name (machine name), URL, or IP address where Forguncy Server is installed. <br/>The computer name can be found in the user account management screen of Forguncy Server Manager.|
|**User Name**|Specify the Forguncy Server username. <br/> Applications can only be published by user accounts that belong to the *Administrator* role or a role to which the **Publish to Server** privilege has been assigned in **Server Manager**. By default, *Administrator* belongs to the *Administrator* role. <br/> ![server-roles-assign-authentication](/assets/images/product-images/server-roles-assign-authentication.png)|
|**Password**|Specify the password for the user. The default password for the default user account *Administrator* is *123456*.|
|**Site Port**|The default port number is *80*. You are allowed to specify the port number if you want to change it. <br/> The port numbers that can be specified are from the default 80 and 1025 to 65534. <br/> If you are publishing to the Linux version of Forguncy Server, the same port number cannot be used by multiple apps. If you try to publish to a port number that is already in use, the system will display an alert message.|
|**Application Name**|Specify the application name. The application name will eventually become a part of the application's URL for the users. The application name is saved with each project file. <br/> Space characters cannot be used at the beginning or end of the application name. <br/> If there are blank characters at the beginning and end of the application name, those blank characters will be automatically deleted on the click of the **Publish** button.|
|**Destination URL**|The URL is generated based on the entered application name. It is a Non-editable filed.|

Note: The server name, port number, and application path determine the destination URL for users to access the application.
{:.note}

Set the below operations as required:

|**Override Database**|When publishing for the first time, all applications and data will be published regardless of this setting. <br/> When republishing, the behavior changes depending on the type of table you are using. <br/> Select the appropriate one for how you would like your development and production environment databases to be. <br/> ![app-publishing-settings-dialog-override-database](/assets/images/product-images/app-publishing-settings-dialog-override-database.png)|
|**Take Server Online After Publish**|Checking this will launch the Forguncy Server online|
|**Publish User Service**|Publish the user account management service information registered in the development environment to Forguncy Server in the operating environment. By default, **Publish Roles to Server** is checked. As per the requirement you can publish users and organizations to Server as well. <br/> ![app-publishing-settings-dialog-publish-user-service](/assets/images/product-images/app-publishing-settings-dialog-publish-user-service.png)|
|**Override UI Permissions to the Server**|Reflects the page display authority and cell access control settings on the Forguncy Server side. <br/> Since the settings on Forguncy Builder are completely overwritten, if you have changed the page display authority or cell access control settings on the Forguncy Server side, those settings will be deleted.|
|**HTTPS**|To use HTTPS. It is necessary to set HTTPS on the Forguncy Server side in advance.|

After completing the above settings, click **Test Connection**.

- Click Publish to publish the application to Forguncy Server. The start page is displayed in your web browser.

Note: If the connection to the database fails and the data does not display correctly, there may be a permission problem. <br/> For Forguncy Server on Windows, the Forguncy Server service process runs under the "Local System" account. <br/> For example, if you are connecting to SQL Server with Windows authentication in your application, the "Local System" account is not valid for Windows authentication, so data cannot be retrieved correctly. In such a case, you need to change the Forguncy Server service login to an account that allows Windows authentication. <br/> For the Linux version of Forguncy Server, the Forguncy Server service process (daemon) runs with root privileges.
{:.note}

- Launch the Forguncy Server Management Portal and verify that your published application is listed.

![app-publishing-launch-forguncy-server](/assets/images/product-images/app-publishing-launch-forguncy-server.png)
{:.dropshadow}

## Firewall inbound rules (port opening)

When an application is published to Forguncy Server or the Forguncy Server service is restarted, Forguncy Server will automatically change the firewall settings to use the port numbers required by the application. 

However, for the Linux version of Forguncy Server, the port opening is a temporary setting and will be disabled when the server is restarted. If permanent port opening is required, reconfigure the firewall for the required port numbers.

