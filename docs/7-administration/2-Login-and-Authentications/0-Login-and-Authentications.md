---
layout: default
title: Login and Authentications
parent: Administration
permalink: /working-with-forguncy-builder/administration/ulogin-and-authentications/
nav_order: 2
has_children: true
has_toc: true
---

# {{ page.title }}

The accessibility of applications build in Forguncy Builder is restricted to authorized users only. In this section you will learn how to control login and authentications of applications. 

In addition, when operating on a server, a concurrent connection license is required according to the number of clients that connect to the application at the same time (per web browser, not per device). So, it is necessary to activate the license first. Read Forguncy [Installation and Deployement](https://docs.forguncy.net/installation-and-deployment/) for the details.

## Advantages of Authentication

Below are the top reasons why you should need authentication for the application.

Compared to applications that do not log in, applications that log in to authenticate users can:

### Protection of information for specific users
Permissions can be set on tables for the most secure protection of the information. Setting permissions such as *Read* and *Edit* for specefic users and roles on a record-by-record and field-by-field basis. In Forguncy, it is also possible to centrally protect information for all the data access, such as pages and web APIs.

For simpler information protection, you can set userwise or rolewise access rights for each page. User accounts that do not belong to a role that allows access cannot display the page.

In addition, by using the **Conditional branch** command, you can divide the processing according to the logged-in user and role. Specifically, it is possible to create a button that can only be clicked by users who belong to a specific role.

### Leveraging User Account Type Fields
In Forguncy's internal database, a table allows you to define a field as *User*, which is the data type used to store Forguncy's user account information.

![User-account-type-fields](/assets/images/product-images/User-account-type-fields.png)
{:.dropshadow}

The user who logs in and uses the application are automatically saved in the user account type field called *User*. If the logged in users are the users from the table field then they can always set the *Last Modified By* field. 

### Audit log
By enabling login to all the pages of an application, audit logs can show you the necessary details about the operations performed in an application by the users. 

### Use of workflow functions
The [workflow](https://docs.forguncy.net/working-with-forguncy-builder/Workflows/#workflows) function is a function that manages the current person in charge and the status of the data in an application. So, in order to actually use this function, it is necessary to register a user account.

### Use of update notification function

![command-send-email](/assets/images/product-images/command-send-email.png)
{:.dropshadow}

By using the *Send Email* command, you can be notified by email when data is updated or changed. This e-mail is sent to the e-mail address that is set for the registered user account. So, it is necessary to register a user account.


The two main types of authentication modes provided by Forguncy are-

## Form Authentication

By default, *Forms Authentication* is set. Since users are authenticated using Forguncy's user management service, it is necessary to register users as form authentication by [adding users](https://docs.forguncy.net/administration/User-service-manager/user/#how-to-add-users) in advance.
When you run the application you will see the user login page. Enter your registered username and password to log in.

<!-- Permission settings such as who can view which page when the application is executed can be achieved by the method described in Setting Page Display Permissions . This default is set to "logged in user". This ensures that the login screen will always be displayed when you run the application with the default settings. If you do not want to display the login screen each time, such as when starting the application frequently for debugging, etc., you can prevent the login screen from being displayed by specifying "Anyone" for the target page. -->

## Windows Authentication

Windows authentication is an authentication method that can be used when a company uses *Active Directory* for user management and logs in using a *Windows* user account from a computer belonging to the company's domain. 

<!--For Windows authentication, you may be able to skip entering the user name and password depending on the type and settings of the web browser. In this case, the application can be used immediately without displaying the login dialog etc.

If you select *Windows Authentication* , *Anyone* will not be displayed in the [Manage Page View Permissions] dialog screen described in Setting Page View Permissions, and "Login User" will be set by default. -->

Note: Only users registered as Windows authentication users of Forguncy can log in to the published application. <br/>However, in Forguncy Builder's debug mode, you can log in even if the user is not registered as a Windows authentication user.
{:.note}