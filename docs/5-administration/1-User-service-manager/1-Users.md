---
layout: default
title: Users
parent: User Service Manager
grand_parent: Administration
permalink: /administration/User-service-manager/user/
nav_order: 1
---

# {{ page.title }}

User means the account that logs into an application. The **Users** menu in User Service Management allows you to add and manage users for the development environment.

![users](/assets/images/product-images/users.png)
{:.dropshadow}

The values ​​of *user name*, *full name*, and *email address* set here are the "%CurrentUser.UserName%", "%CurrentUser.FullName%", and "%CurrentUser.Email%" keywords for data acquisition respectively. 

For example, if you write "%CurrentUser.UserName%" in a cell, it will be displayed as "Administrator" if you log in as the default Administrator.

The following buttons are clickable only if the action is valid.

![user-management](/assets/images/product-images/user-management.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|Add User|Allows you to add users. It can be either form users or windows users.|
|View Settings|Allows you to set visible columns. Items that are checked are displayed. The extended attributes are also displayed here.|
|Remove Users|Allows you to remove multiple users. Check the checkbox of the user(s) you want to delete and then click this button. Administrator users cannot be deleted.|
|Edit User|Check the checkbox of the user you want to edit and then click this button. Only single selection is allowed. You can also hover the mouse on the user record and click the Edit button.|
|Edit User Role|Check the checkbox of the user whose role you want to change and then click this button. You can also hover the mouse on the user record and click the Edit User Role button.|
|Reset Password|Check the checkbox of the user whose password you want to change and then click this button. You can also hover the mouse on the user record and click the reset Password button. The password must be 6 or 18 characters.|
|Search|Enter a value in the search box and press the Enter key or click search to find *user name*, *full name*, *email address*, and *role*. The corresponding information is displayed in the user list.|
|Sort|Click the title of the user list to sort in descending or ascending order.|

## How to Add Users

Describes how to add users using the user account management screen during development. same applies to the server management portal during operation.

- Select Internal Administration , Users, and click the Add User button.
- Select an authentication method and add users.
    "Forms authentication" and "Windows authentication" users can be added together. However, the authentication method that can be used in one application is limited to the users specified in Setting the user authentication mode .

If you have created extended attributes, they will appear at the end of the Add User screen below so that you can assign extended attributes to users. For example, you can create "supervisor" in the extended attribute, and specify Mr. B as Mr. A's superior when adding user A here.

### How to add a "Forms Authentication User". 
Click the Forms Authentication Users tab as shown below. Enter the information according to the display and click the "OK" button to complete the addition.
### How to add a "Windows Authentication User"
- Click the "Windows Authentication Users" tab as shown below. <br/>Switch between automatic and manual domain synchronization
By default, Forguncy tries to pick up new Windows authenticated users added on the domain and automatically syncs them. You can get the latest information by clicking the [Update to the latest Windows authentication user information] button in the red frame on the screen below.<br/>Forguncy has an expiration time of 5 minutes to automatically retrieve user information from your domain. If the network environment is slow, it may take 3 minutes to acquire. You can switch this to manual sync by changing "AutoSyncWindowsDomainUsers" in the file below to false. See Global Settings for more information on this. File Location: C:\Users\Public\Documents\ForguncyServer\GlobalConfig.xml
-  Enter a value in the search box and press the Enter key or click to perform a search and display a list of search results according to the entered content. If you don't enter a value in the search box, the domain's users will be displayed in the full list. Note that users who have already been added as Forguncy users will not be displayed in the list. <br/>Here, check the user you want to add and click "OK". You can check multiple people at once. The value entered in the search box is searched for "user name", "full name", and "email address" in a case-insensitive manner.
- You can confirm that the user has been added to the list as shown in the screen below.



