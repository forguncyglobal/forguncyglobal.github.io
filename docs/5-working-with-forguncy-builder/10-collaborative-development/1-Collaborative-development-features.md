---
layout: default
title: Collaborative Development Features
parent: Collaborative Development
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Collaborative-development/collaborative-development-features/
nav_order: 1
---

# {{ page.title }}

To access collaborative development features, go to **Advanced** tab -> **Collaborative Development** section. There are following controls available for the collaborative development:

|Controls|Description|
|:--|:--|
|**New Git Repository**|Upload the currently open project to Git server and create a new team development project on the server side. For private repositories, login is required the first time you connect. If so, enter your username or email address and password.|
|**Open Git Repository**|Enter the Git repository URL to open an existing team development project. For private repositories, login is required the first time you connect. If so, enter your username or email address and password.|
|**Modules**|The Modules dialog lists all modules in your project and their status, allowing you to see who checked out and when modules were modified.|
|**Pending Changes**|It will list all the changes you have made. Developers can check in or undo all changes made from this dialog. <br/><br/> Check In: ​​Commit module changes to the Git repository. <br/> Revert: Revert all changes and revert to the latest version on the Git repository. <br/><br/> There are two categories of modules: changes to be included in check-in and changes to be excluded from check-in. <br/> Changes to include in check-in: By default all changes are displayed in this category. Enter your comment in the text box and click the Check In button to check in all modules in this category. <br/> Changes Excluded from Checkin: If you want to check in only some of the module changes that do not need to be checked in, click [Exclude] on the context menu and select the [Changes Excluded from Checkin] category. Go to.|
|**History**|All changes are listed in this dialog. Right-clicking a changeset displays a context menu that allows you to <br/> <br/> Rollback to this version: Restores the current project to the selected version. All modules must be available for checkout to perform this operation. <br/> <br/> Save this version as Forguncy file...: Saves the selected version as a Forguncy file (FGCP file). <br/> Copy changeset ID to clipboard: The changeset ID can be used to uniquely identify the change history, such as in searches.|
|**Get latest Version**|Get the latest version of the server. Click the dropdown button to select either Get latest or Discard pending changes and get latest. <br/> Get Latest: Gets the latest version of the server without discarding any changes made in the currently open project. <br/> Discard Pending Changes and Get Latest: Discards any changes you have made in the currently open project and gets the latest from the server.|
|**Settings**|You can set or change your user name and email address. The username set here will be displayed in the revision history. This username and email address will be used for check-out and check-in. By default, the user name is set to the Windows login user name or the Windows computer name. <br/><br/> The authentication information entered in this dialog is automatically saved for each Windows user, and entry is not required for subsequent connections. If you want to remove and reset your credentials, click Clear All Credentials and your credentials will be cleared. Note that if you had credentials stored for multiple different Git hosting services, they will all be deleted and reset.|
