---
layout: default
title: Version 8.1
parent: Releases
permalink: /releases/version-8.1/
nav_order: 1
---

# {{ page.title }}

Forguncy Builder 8.1 has following changes:

### Cell Types

- In button cell type, there are added options of adding Left Icon and Right Icon, instead of a single icon.
- Available operations in button cell type (right pane)
    - Set Left Icon
    - Set Right Icon
- In Radio group cell type, extra available operation - Clear Other Text
- New cell type - UserControl Container

### Reports

- In 'Add Data Source' dialog of Report, in the 'Add Column' button, there is a dropdown with the provided option of 'Add all columns', which adds all columns at once. 

### Security

- In File Tab->Options->Application Settings-> Security section - There is an added option - 'Do not allow to query the database by JavaScriptAPI'.

### Commands

- New command in Flow Control section - 'BreakCommand'
- 'SetCurrentRowCommand' is removed.
- New section of commands - Server Notification (2 commands)
- 'Start Loading' and 'End Loading' commands are removed. 
- When 'Invoke Cell Type Operation' command is applied on the 'button' cell type, it gives the options to perform operations 'Set Left Icon' and 'Set Right Icon'.
- In 'Update Data Table' Command's advanced settings, there is an extra option asking whether to 'Update consolidated data to the latest information'.
- In 'Call Stored Procedure' command, there is an extra option asking whether to 'Update consolidated data to the latest information'.

Forguncy Builder 8.1 has following changes:

### Server Manager

- In Forguncy Server manager->Settings->Configurations - 2 new configurations are added - 'Cloud Storage Settings' and 'Log'.
- Forguncy Server Manager-> Settings -> Configurations ->Account Security->Addition of two new Password policies
- Forguncy Server Manager-> Settings -> Configurations ->Windows Domain User Sync - Addition of 'Domain User Filtering settings'.
- Administrator dropdown - Added option of 'Change Password'. (three dots in upper right corner)

### Others

- User Control (see in 'Create' ribbon tab)
- Server Notification (see in 'Create' ribbon tab)
- Mobile Debug option (see in 'Debug' section in 'Home' ribbon tab)
- In 'Data' ribbon tab-> Manage Connections - The dialog that opens up, has some UI changes, and there is an additional option of import/export file.
- In the Data Validation dialog-> Error Alert section - There is an added option of whether to show error alert on 'errortip' or 'cell'.

Other than the above changes, there are changes in field names and labels (nomenclature) at various places.