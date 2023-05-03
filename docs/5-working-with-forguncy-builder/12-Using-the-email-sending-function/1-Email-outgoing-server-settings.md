---
layout: default
title: Email Outgoing Server Settings
parent: Using the Email Sending Function
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Using-the-email-sending-function/Email-outgoing-server-settings/
nav_order: 1
---

# {{ page.title }}

Configure the settings for the mail sending server that are required when debugging an application that uses the function to send mail. 

To use the e-mail sending function, a mail server that can use SMTP is required. If you do not have an e-mail server, you can use a webmail service or an email delivery service.

Note: The mail sending server settings set on Forguncy Builder during application development will not be carried over to the production environment. It needs to be reconfigured on the server management portal of Forguncy Server.
{:.note}

For SMTPs over SSL/TLS, specify 465 as the port number. SMTPS on port numbers other than 465 is not supported. For other than SMTPS (such as STARTTLS), specify the port number recommended by the mail delivery service, such as port number 587 or 25.

The steps of the server settings using the user account management screen during development are explained below. The same applies to the server management portal during operation.

- Open **User Service Manager** and go to **Settings**.
- Click **SMTP** settings.

![user-service-manager-smtp-settings](/assets/images/product-images/user-service-manager-smtp-settings.png)
{:.dropshadow}

- Enter values ​​in the required items and set the mail transmission server.

Note: Check **Enable SSL** if your SMTP server uses SSL or TLS for transmission.
{:.note}

- Click the **Send Test Email** button to test your mail server settings.
- Click the **Save** button to save your settings.