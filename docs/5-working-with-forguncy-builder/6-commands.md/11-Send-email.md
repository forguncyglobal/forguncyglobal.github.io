---
layout: default
title: Send Email
parent: Commands
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/commands/Send-email/
nav_order: 11
---

# {{ page.title }}

This command allows to send any content as mail. 

Note: The mail server (SMTP outgoing server) must be set before using this command. For both the application development environment and the Forguncy Server production environment, please refer to [Email Outgoing Server Settings]().
{:.note}

![command-send-email](/assets/images/product-images/command-send-email.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|**From**|To enter the sender's email address. The values ​​that can be set are: <br/> - Sender email address string <br/> - Forms authentication user "username" <br/> - Formulas that refer to cell values. <br/> *Note: When using the send email command from the "Command" button in the workflow settings , please note that including cell references on the page in the formula may cause unexpected behavior due to dynamic changes in the page.* <br/> - Keywords can be used such as %CurrentUser% : logged in user|
|**To**|To enter the recipient's email address. The values ​​that can be set are: <br/> -Recipient email address string. When specifying multiple recipients , separate each email address with a comma **,**. <br/> - Forms authentication user "username". When specifying multiple recipients, separate each email address with a comma (,). <br/> Formulas that refer to cell values. <br/> *Note: When using the send email command from the "Command" button in the workflow settings , it is not recommended to include cell references on the page in the formula as it will behave unexpectedly when the page changes dynamically.* <br/> - Keywords can be used such as %CurrentUser%: logged in user. <br/> when using the Send Email command from the "Commands" button in the workflow settings then <br/> - %ReleatedAssignTo%: Related approver. If there are 3 approvers (A, B, C), send to 3 people. If A is approved, I will send it to B and C. <br/> - %HistoryPartner%: People included in the history of the workflow <br/> - %AssignTo%: the next assignee <br/> - %Creator%: creator <br/> - %LastModifier%: Last modified by|
|**Subject**|To enter the email subject. The values ​​that can be set are: <br/> - A string that will be the subject. <br/> - You can use a formula in the subject line by clicking However, when using the send email command from the "Command" button in the workflow settings , it is not recommended to include cell references on the page in the formula, as it will behave unexpectedly when the page changes dynamically. <br/> - Keywords can be used.|
|**Content**|To enter the body of the email. The values ​​that can be set are: - Content string. <br/> - Since the email to be sent will be in HTML format, the character string can use tags that can be used in general HTML format emails. <br/> - If you check **Use formula for content**, you can write the text in formulas. <br/> When this check is enabled, the entire body of the email must be written as a formula. This check is automatically disabled if a value that is not a formula is entered. <br/> *Note: when using the send email command from the "Command" button in the workflow settings , it is not recommended to include cell references on the page in the formula, as it will behave unexpectedly when the page changes dynamically.* <br/> - Keywords can be used. <br/> ![command-send-email-edit-mail-content](/assets/images/product-images/command-send-email-edit-mail-content.png)|

You can configure the following settings by clicking **Show advanced settings...**.

|**CC**|To specify a CC email address. When specifying multiple CCs, separate each email address with a comma **,**. You can also enter formulas.|
|**BCC**|To specify a BCC email address. When specifying multiple BCCs, separate each email address with a comma **,**. You can also enter formulas.|
|**Attachment**|To send files as email attachments. Separate multiple attachments with vertical bar.|
|**Priority**|To specify the importance of the mail as *Low*, *Normal*, and *High*|
|**Send as Plain text**|If you check this check option, the email will be sent in plain text format. If not checked, a multipart email with both HTML formatted data and text formatted data will be sent. Default is disabled. <br/> In the case of an application that allows you to enter the text of the email to be sent, or part of the text, from a web page using cell references, etc., it is recommended to send the text in text format instead of HTML format.|

Note: It is also possible to use a cell reference as the destination and set the reference to a *User Selector* cell type.
{:.note}