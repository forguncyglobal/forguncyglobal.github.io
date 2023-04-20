---
layout: default
title: Collaborative Development
parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/collaborative-development/
nav_order: 10
has_children: true
has_toc: true
---

# {{ page.title }}

Forguncy provides features for multiple developers to collaborate and manage the same project. It supports collaborative development for large-scale apps with high flexibility and efficiency. 

## Collaborative Development Overview

### Check Out and Check In

Check out and check in are the most basic concepts in Forguncy collaborative development. Check out and check in prevents multiple developers from editing the same module at the same time and causing conflicts.

- **Check Out**: Locks the module from being edited by other users and can only be edited by the developer who checked it out.
- **Check In**: ​​Integrate the changes in a checked out module, unlock it and make it available for other developers to check out.

### Module

A module is the smallest unit that can be checked in or checked out in Forguncy. Each page is a module. It is necessary to check out the database and perform the **Refresh** operation to reflect changes.

- Database
- Page
- Master page
- Server side command
- Schedule task
- Report
- Application settings
- Theme
- Import image
- User account
- Custom library
- Reuse command
- GeoJSON file
- External database connection information
- Upload file

### Git

Git is generally one of the version control systems for recording and tracking the change history of program source code, etc., and is provided as open source software. Besides installing Git on your local network to build a Git server, several companies deploy Git hosting services.

In order to use Forguncy's collaborative development features, you'll need to enable a Git repository first.

## Precautions when using the Collaborative Development Function

- Forguncy uses WinHTTP to connect to Git servers. This is different from WinInet, which web browsers use. Therefore, if the environment uses a proxy server, WinHTTP communication must be configured to go through the proxy server.

- There is an upper limit for Git repository size and file size to upload. See Forguncy Specifications and Limitations for more information. The Git system may store multiple files as a single binary file called a "packfile". For example, if you use the Download Registration Files command to include multiple large files in your project, they will be converted to a "packfile" even if the single file size does not exceed the limit. may exceed the limit.

- When using plugins, all developers must install the same version of the plugin in each environment (Forguncy Builder). An error is raised if this is not the case.

- Since it is easier for different users to be in charge of different parts in the early stages of application development, using this function improves development efficiency.

- Before starting application development, design the interface and style of the application, and design the style to use more elements on the UI such as buttons, tables, etc. By doing so, the developer can unify the styles by simply applying the styles prepared during application development.

- A database is a module that cannot be checked out by another developer while one developer is modifying it. An inconsistent database can greatly affect development efficiency, so it's a good idea to design your database in advance and ensure that changes are made only by the people responsible for maintaining the database.

The following features are not available in collaborative development projects.

- Data Ribbon Tab-> From Forguncy Project
- Create Ribbon Tab-> Generate Pages and Tables from Excel

- Start page settings are unmanaged. The start page during operation is set to the page (active sheet) that is open in Forguncy Builder by the app publisher when it is published. If no page is open, Forguncy will randomly set a valid page as the start page.