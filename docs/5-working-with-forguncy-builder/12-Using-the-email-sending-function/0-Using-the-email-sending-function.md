---
layout: default
title: Using the Email Sending Function
parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Using-the-email-sending-function/
nav_order: 12
has_children: true
has_toc: true
---

# {{ page.title }}

When using Forguncy's function to send the following emails, it is necessary to set the outgoing mail server in advance. In addition, since the "Password reset guide mail" and the "[E-mail notification registration] command" are sent to the e-mail address set for the registered Forguncy user, please do not send these e-mails. User authentication function is required to use the function.

- To use the e-mail sending function, a mail server that can use SMTP (Simple Mail Transfer Protocol) is required.
- When testing the function to send emails in the application development environment, it is necessary to set the SMTP transmission server on the Forguncy Builder side. Also, when running an application that uses the function to send emails on Forguncy Server, it is necessary to set the SMTP transmission server on the Forguncy Server side

### Password reset guide email
A password reset guide email will be sent to users who have forgotten their login password. See What to do if a user forgets their password for details .

### Register for Email Notification Command
By using the email notification registration command, when an addition or change is made to the target table, a change notification email will be automatically sent to the user who wishes to be notified .

### Send E-mail command
Any content can be sent as an email by using the email sending command.

### SendMail method
Send an email by specifying the destination, email title, and text from JavaScript.