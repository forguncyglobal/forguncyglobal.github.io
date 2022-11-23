---
layout: default
title: Single Sign On
parent: Administration
permalink: /administration/Single-sign-on/
nav_order: 3
---

# {{ page.title }}

Single sign-on enables users to automatically log in to the Forguncy website with the application credentials on switching between application and website.

## The schematic diagram of single sign-on 

![schematic diagram of single sign-on](/assets/images/product-images/)
{:.dropshadow}

### GetUserToken interface description
**Request method**

Post

**Parameter**

|Parameter|Description|
|:--|:--|
|UserName|Username required to log in|
|Password|Single sign-on password|

**Return value**

string. If the token acquisition succeeds, the returned string does not start with "Error:"; if the token acquisition fails, the returned string is the error message and starts with "Error:", which is convenient for debugging and positioning.

Note: The username must exist in the movable type user management system.
{:.note}

### Use Cases

- When existing Application navigate to ForguncyPage, The ForguncyPage will be login as existing Application's User.
- The user can login the page by the existing Application's user name and password.

## Steps to set up single sign-on

In the Forguncy Builder, select "File -> Settings -> Integrate with another website" to view and set the password for single sign-on. See Table 1 for setup instructions.

![single sign-on-builder](/assets/images/product-images/single-sign-on-builder.png)
{:.dropshadow}

|Parameter|Description|
|:--|:--|
|Allow single sign-on| Whether to enable single sign-on, it is not enabled by default, and the value is False.|
|Single sign-on password| The password required to obtain the user token. <br/>A password is randomly generated when the designer is opened. After allowing single sign-on, if you do not save the file, the password will be regenerated the next time you open it; if you save the file, the password will not change when you open it again.|
|Token timeout time| Token validity time|

After setting up single sign-on, write the following code in the third-party (non-movable type) application-

**C# Example**

![single sign-on c# code](/assets/images/product-images/single-sign-on-c%23-code.png)
{:.dropshadow}


## How to change the password without republishing

- Use Path **C:\Users\Public\Documents\ForguncyServer\[AppName]\Config.xml** and open the config file of an application in the server. 
- Go to password node to change.

Note: The empty password node represents the builder password. 
{:.note}

- After making changes, restart the website.

![single sign-on change password](/assets/images/product-images/single-sign-on-change-password.png)
{:.dropshadow}