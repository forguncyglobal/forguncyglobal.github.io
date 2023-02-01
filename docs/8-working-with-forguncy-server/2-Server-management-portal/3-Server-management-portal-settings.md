---
layout: default
title: Server Management Portal Settings
grand_parent: Working with Forguncy Server
parent: Server Management Portal
permalink: /working-with-forguncy-server/server-management-portal/server-management-portal-settings/
nav_order: 3
has_children: false
has_toc: false
---

# {{ page.title }}

The Settings menu of the Server Management Portal allows you to configure the following settings:

![forguncy-server-manager-settings](/assets/images/product-images/forguncy-server-manager-settings.png)
{:.dropshadow}

|**SMTP Settings**|To set the mail transmission server.|
|**Account Security**|To configure password policy and two-factor authentication settings.|
|**Backup and Restore**|Allows you to automatically back up your applications and user account information on a regular basis.|
|**Windows Domain User Sync**|User information that has been changed on the Active Directory side is automatically reflected in Windows authentication user information on the Foguncy side. <br/> This function does not exist in the Linux version of Forguncy Server.|
|**HTTPS Certificate**|You can enable HTTPS communication for your Forguncy application and Forguncy server management portal.|
|**Storage Path**|Various paths can be specified, such as the folder where the Forguncy application is placed and the folder where the audit log is saved.|
|**Web Security Policy**|To configure security settings that affect the Forguncy Server Management and all applications running on Forguncy Server.|
|**Database Config**|To configure the User Account Information Database. You can change the storage destination of user information to MySQL and SQLServer.|