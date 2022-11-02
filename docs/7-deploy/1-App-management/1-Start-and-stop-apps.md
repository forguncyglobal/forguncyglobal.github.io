---
layout: default
title: Start and Stop Apps
parent: App Management
grand_parent: Deploy
permalink: /deploy/app-management/start-and-stop-apps/
nav_order: 1
---

# {{ page.title }}

Applications published to the server must be started before users can access them.

Also, when performing database maintenance using the "Obtain operational database" function, the application must be put into maintenance mode or stopped.

To start and stop the application from the Forguncy Builder side, use the "Release maintenance mode" and "Release maintenance mode" functions. When set to maintenance mode, the "FGC_Maintenance now" built-in page will be displayed.

## Cancel maintenance mode

If you check the "Remove maintenance mode after publishing" checkbox when publishing the application, the maintenance mode will be automatically canceled. If you issue without checking and the application on Forguncy Server is set to maintenance mode, you need to cancel maintenance mode by the following method.

- Click the [Publish] ribbon tab of Forguncy Builder > [Release Maintenance Mode] button.
- Make sure the server settings are correct and click OK.

|Server|Specify the computer name (machine name), URL, or IP address where Forguncy Server is installed.|
|Username|Specifies the Forguncy Server username. Please note that I am not a Windows user. <br/> Maintenance mode can only be canceled by user accounts that belong to the "Administrator" role in user account management or to a role that has been assigned the "Publish application to server" privilege. By default, "Administrator" belongs to the "Administrator" role.|
|Password|Specifies the password for the user. The default password for the default user account "Administrator" is "123456".|
|Application name|Specify the name of the application whose maintenance mode you want to release. The application name can be finally confirmed from the destination URL of the application used by the user.|

Note: Click [Check Connection] to test the connection with Forguncy Server.
{:.note}

## Set to maintenance mode

Put the application in maintenance mode and make it inaccessible to users. When users access the application at this time, they will see the following screen notifying them that it is under maintenance and the application will be unavailable.

Note: You can edit the maintenance notice page. See built-in page for details.
{:.note}

- Click the Publish ribbon tab in Forguncy Builder > Set to Maintenance Mode button.
- Make sure the server settings are correct and click OK.

|Server|Specify the computer name (machine name), URL, or IP address where Forguncy Server is installed.|
|Username|Specifies the Forguncy Server username. Please note that I am not a Windows user. Only user accounts belonging to the "Administrator" role or a role to which the "Publish application to server" privilege has been assigned in user account management can be set to maintenance mode. By default, "Administrator" belongs to the "Administrator" role.|
|Password|Specifies the password for the user. The default password for the default user account "Administrator" is "123456".|
|Application name|Specify the application name that you want to set to maintenance mode. The application name can be finally confirmed from the destination URL of the application used by the user.|

Note: Click [Check Connection] to test the connection with Forguncy Server.
{:.note}

## Starting and stopping from Forguncy Server
To start and stop the application from the Forguncy Server side, use the "Start" and "Suspend" functions. If you stop the app using this feature, accessing the application will now display the HTTP 404 error page.

### App start

- Follow the Server Management Portal procedure to display the Server Management Portal screen.
- Select [Apps] and click the start icon of the target application from the list of applications. The user will be able to access the application. Note that if the application has already started, this button will display an interrupt icon.

### stop app
- Follow the Server Management Portal procedure to display the Server Management Portal screen.
- Select [Apps] and click the stop icon of the target application from the application list. Users will no longer be able to access the application. Note that if the application has already been stopped, this button will display a start icon.