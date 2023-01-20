---
layout: default
title: Loading and Running the Project
parent: Project
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Project/loading-and-running-the-project/
nav_order: 4
---

# {{ page.title }}

## Loading a Project

To open a saved project, go to **File** and click **Open**.

![project-open-project](/assets/images/product-images/project-open-project.png)
{:.dropshadow}

|Recent|A list of recently opened projects appears on the right. You can select and open it from here.| 
|Browse|The **Open** dialog appears where you can search for the required project.|
|Git Repository|An **Open Project from Git Repository** dialog appers where you can enter the URL of the Git repository and select branch.|

If the opened project contains plug-ins that have not been installed in this environment, or if the version of the plug-ins installed in this environment is old, a dialog will be displayed and the plug-ins required for the opened project will appear. You can install from there.

Note: <br/> Projects created with an older version of Forguncy Builder will be converted and loaded when opened with a newer version of Forguncy, but projects created with a newer version of Forguncy cannot be opened with an older version.<br/><br/> Forguncy supports projects saved in the previous two major versions of Forguncy Builder. Projects created with older versions may not work properly even if they can be opened.<br/><br/> The same project file cannot be opened in multiple Forguncy Builders. If you do so, Forguncy Builder, that already has that project file open will be brought to the front.
{:.note}

## Running a Project

The project can be run by either of the following operations, and you can check the results immediately. Read [Run and debug]() for more details.

- Go to **Home** tab.
- Click the **Start** button (green triangle icon).

![project-run-project](/assets/images/product-images/project-run-project.png)
{:.dropshadow}

- The following login screen will be launched by default. If you do not want to display this screen then you can [disable the login screen](#disable-login-screen).

![project-run-project-signin-screen](/assets/images/product-images/project-run-project-signin-screen.png)
{:.dropshadow}

### Disable login screen
During development, if you do not want to display the login screen to check the operation, you can disable it as follows-

- Go to **Security** tab and click the **Authority Management** option.
- On the **Authority Manager Window** set unrestricted page permissions to *All*. 

![project-disable-login-screen](/assets/images/product-images/project-disable-login-screen.png)
{:.dropshadow}

Read [Page permissions](https://docs.forguncy.net/administration/login-and-authentications/page-permission-and-cell-access-control/) for more details.
