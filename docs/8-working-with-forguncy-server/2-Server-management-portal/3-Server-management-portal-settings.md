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
|**Backup and Restore**|Allows you to manually or automatically back up your applications and user account information on a regular basis.|
|**Windows Domain User Sync**|User information that has been changed on the Active Directory side is automatically reflected in Windows authentication user information on the Foguncy side. <br/> This function does not exist in the Linux version of Forguncy Server.|
|**HTTPS Certificate**|You can enable HTTPS communication for your Forguncy application and Forguncy server management portal.|
|**Storage Path**|Various paths can be specified, such as the folder where the Forguncy application is placed and the folder where the audit log is saved.|
|**Web Security Policy**|To configure security settings that affect the Forguncy Server Management and all applications running on Forguncy Server.|
|**Database Config**|To configure the User Account Information Database. You can change the storage destination of user information to MySQL and SQLServer.|

## Backup and Restore 

You can backup application data and user information either manually or automatically. 

Manual backup is done by the **Backup Now** button. It is a one-time procedure. You need to simply click the button to initiate the process. 

The automatic backup process can be schedulled and run on a regular basis. Enable **Scheduled Backup** and fill in th required details. 

You are allowed to set the backup folder. The default backup location is *C:\Users\Public\Documents\ForguncyServerBackup*. Folder path can be a shared path of another computer such as "\\another-PC\Shared\"

Note: It is recommended to select shared folder so just in case the Forguncy server breaks down, you can always locate the backup file from the other computer.
{:.note}

All the backups are listed under **Backups** section. Expand the record to view details. You can perform operations like *Restore*, *Download*, or *Delete* as per the requirement. 

![forguncy-server-manager-backup](/assets/images/product-images/forguncy-server-manager-backup.png)
{:.dropshadow}

The backup file name will be in the following format:

- App: "manual-yy-MM-dd-hh-mm-ss.fdbak"
- User information: "usersBackup-manual-yyyy-MM-dd-hh-mm-ss.fubak"
- Global Settings: "GlobalConfig-manual-yyyy-MM-dd-hh-mm-ss.fubak"

* The date is set in [yyyy-MM-dd-hh-mm-ss].

## Synchronization of Windows Authenticated Users

To use a Windows user in Active Directory as a Forguncy user account, use **Windows Domain User Sync**. It allows you to register a Windows user as a Forguncy user.

This sync obtains not only user account information, but also roles and organizations information from the Active Directory. When there are any changes on the Active Directory side, the information reflects here automatically.

![forguncy-server-manager-windows-domain-user-sync](/assets/images/product-images/forguncy-server-manager-windows-domain-user-sync.png)
{:.dropshadow}

Note: This feature only exists for the Windows version of Forguncy Server. It is not displayed in the Linux version of Forguncy Server.
{:.note}

**Domain User Filtering Settings** allows filtering of Windows domain users based on the organization filter settings when synchronising.

You can either run manual sync by clicking the **Manual Sync** button or enable automatic sync by checking **Enable Sync** and do the required settings.


