---
layout: default
title: Subscribe
parent: Commands
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/commands/Client-side-commands/Subscribe/
nav_order: 12
---

# {{ page.title }}

If you subcribe for email notification, a change notification email will be automatically sent to the registered user when there is a change (addition, modification, or deletion) in the target table.

Read [Commands](https://docs.forguncy.net/working-with-forguncy-builder/commands/) to understand command execution steps.

Subscribe command only supports email notification for single record addition, modification, and deletion. If multiple records are updated by one process, email notifications will not be sent by this command. However, you can set multiple fields of a record to be notified in the same email. 

Note: The mail server must be set before using this command. Refer [Email Outgoing Server Settings]() for the steps. 
{:.note}

![command-subscribe](/assets/images/product-images/command-subscribe.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|**Subscribed View Name**|To set the name described in the subject of the notification email.|
|**Table**|To select the table for which notification emails will be delivered. <br/> By checking the **Enable View Query** check box, you can set detailed conditions for sending emails.|
|**Columns in View**|To set the field that refers to the value described in the notification email.|
|**Email Settings**|On clicking **Show Advanced Settings**, you can set the sender's email address, recipient's email address, prefix attached to the subject. <br/> If you do not enter sender's email address, the mail sender information set in the [Email Outgoing Server Settings]() will be applied.|