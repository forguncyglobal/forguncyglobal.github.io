---
layout: default
title: User Service Management
parent: Administration
permalink: /administration/user-service-manager/
nav_order: 1
has_children: true
has_toc: true
---

# {{ page.title }}

You can restrict the application usage by user, role, and organization in Forguncy. The Forguncy's user management system allows you to manage users and enable the approval process according to your defined [workflow](https://docs.forguncy.net/working-with-forguncy-builder/Workflows/#workflows).

Depending on the usage and requirement you can manage users from below two locations: 

### User Service Manager

Allows you to manage users on the development environment. It helps in checking the execution result based on different users while debugging the application. It has nothing to do with the user management on the server side. 

Since this setting is saved for respective applications, it is necessary to set each time whenever a new project file is created. When you log in, you will see the user service management screen with a **green** screen style.

### Server Manager

Allows you to manage users on the production environment. User management is available as a part of the server management portal. When you log in, the user account management screen with a **dark blue** screen style will be displayed.

Note: Setting one or the other does not cause both to be set.
{:.note}

- The email transmission server information set in the development environment cannot be carried over to the production environment.
- Role information, user account information, and organization information set in the development environment can be inherited using the publishing function of the Forguncy application.
- User information set in the development environment can only be transferred using the user account information backup and restore function. 


To manage users, roles, and organizations using **User Service Manager** follow the below steps:

- Log in to Forguncy builder and go to **Security** tab.
- Click **User Service**.

![user-service](/assets/images/product-images/user-service.png)
{:.dropshadow}

- Enter cridentials to log in. 

Log in with Forguncy's default administrator account (Username: Administrator and password: 123456). You can change your password if necessary.

![user-service-manager-login](/assets/images/product-images/user-service-manager-login.png)
{:.dropshadow}

- The **User Service Manager** screen will be displayed. In the left pane, under **Security** tab you can manage *users*, *roles*, *levels*, and *organization*. 

![user-service-manager-screen](/assets/images/product-images/user-service-manager-screen.png)
{:.dropshadow}

Note: Information registered in the development environment is for debugging. It will not be reflected on the operating environment of Forguncy Server. During operation, it is necessary to register user information from the " Server Management Portal " on the Forguncy Server side.
{:.note}