---
layout: default
title: Explore the Forguncy Server Manager
grand_parent: Working with Forguncy Server
parent: Server Management Portal
permalink: /working-with-forguncy-server/server-management-portal/explore-the-forguncy-server-manager/
nav_order: 1
has_children: false
has_toc: false
---

# {{ page.title }}

Steps to access the Forguncy Server Management Portal are as follows:

## For Windows version of Forguncy Server

- Click windows **Start** and double-click the **Forguncy Server Manager** icon.

Note: If your environment uses a proxy server, you will not be able to access the Server Management Portal unless the Bypass proxy server for local (intranet) addresses check option is enabled.
{:.note}

- The login screen of the **Forguncy Server Manager** is displayed on the web browser.

![forguncy-server-manager](/assets/images/product-images/forguncy-server-manager.png)
{:.dropshadow}

## Common method for Linux and Windows version of Forguncy Server

- Enter the following URL into your web browser's address bar: 
http://<server name or IP address>:22345/UserService/ManagementPage/LoginPage 

- The login screen of the **Forguncy Server Manager** is displayed on the web browser.

![forguncy-server-manager](/assets/images/product-images/forguncy-server-manager.png)
{:.dropshadow}

## Login to Forguncy Server Manager

Steps to login Forguncy Server Manager are:

- Forms-authenticated users can log in to the Forguncy server Manager with admistrator username and password. However, It is not possible to log in as a Windows authenticated user.

Note: The default administrator credentials are- Username: Administrator and Password: 123456 <br/> You can change your password if necessary. 
{:.note}

- The server management portal screen is displayed.

![forguncy-server-manager-landingpage](/assets/images/product-images/forguncy-server-manager-landingpage.png)
{:.dropshadow}

## Loging off from the Forguncy Server Manager

- Click the username or three dots on the top right corner.
- Select **Sign out** from the drop-down list.

![forguncy-server-manager-signout](/assets/images/product-images/forguncy-server-manager-signout.png)
{:.dropshadow}

## Restarting the Forguncy Server Management Service

- Click the username or three dots on the top right corner.
- Select **Restart Service** from the drop-down list.

![forguncy-server-manager-restart-service](/assets/images/product-images/forguncy-server-manager-restart-service.png)
{:.dropshadow}

- When the reboot is complete, you will be redirected to the login screen.

![forguncy-server-manager-signout](/assets/images/product-images/forguncy-server-manager-signout.png)
{:.dropshadow}

## Forguncy Server Management Menu

The Forguncy Server Management menu allows you to configure the following settings:

|User|To create and edit users.|
|Roll|To create roles and manage role members.|
|Organizational level|To create and manage organizational levels.|
|Organization|To create organizational structures and manage organizational members.|
|Custom Fields|To create and manage extended attributes.|


