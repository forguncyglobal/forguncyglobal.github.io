---
layout: default
title: Send Notification Email When Data Is Updated
parent: Using the Email Sending Function
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Using-the-email-sending-function/Send-notification-email-when-data-is-updated/
nav_order: 2
---

# {{ page.title }}

Use the [Subscribe]() command to set the function to automatically send notification emails when data is updated. 

Since the e-mail is sent to the e-mail address of the registered user account, it is necessary to use a user account to use this function.

- After configuring mail server settings, add **Subscribe** command to a button.

![command-subscribe](/assets/images/product-images/command-subscribe.png)
{:.dropshadow}

- Set up subscription details. 

The user of the application can select and set whether or not to receive the email notification for respective user accounts. Make the selected cell a [Current user](https://docs.forguncy.net/working-with-forguncy-builder/Cell-types/current-user/) cell type, so that you can use the user authentication mechanism. 

![currentuser_celltype](/assets/images/product-images/currentuser_celltype.png)
{:.dropshadow}

If you are not logged in and try to execute the [Subscribe](https://docs.forguncy.net/working-with-forguncy-builder/commands/Client-side-commands/Subscribe/) command, you will automatically be redirected to the login screen and prompted for authentication.

Read [Administration](https://docs.forguncy.net/administration/) to understand Forguncy's user management service and authentication.

Debug to check the operation.

- Log in as *Administrator* and execute the [Subscribe](https://docs.forguncy.net/working-with-forguncy-builder/commands/Client-side-commands/Subscribe/) command.
- Select Notify me on all changes and click OK.
- An e-mail will be sent to the e-mail address set in *Administrator* indicating that the notification settings have been completed.
- Edit the table in your application using the [Update Table Data](https://docs.forguncy.net/working-with-forguncy-builder/commands/Client-side-commands/update-data-table) command.
- Confirm that the notification e-mail has been sent to the e-mail address set for *Administrator*.