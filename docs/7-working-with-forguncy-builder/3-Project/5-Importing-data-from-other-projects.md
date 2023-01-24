---
layout: default
title: Importing Data from Other Projects
parent: Project
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Project/Importing-data-from-other-projects/
nav_order: 5
---

# {{ page.title }}

You can import data for tables, pages (including master pages), reusable commands, server-side commands, and scheduled tasks from existing project files (FGCP files).

Steps to import data from other projects are as follows-

- Go to **Data** tab and click **Forguncy Project**.

![project-import-other-project](/assets/images/product-images/project-import-other-project.png)
{:.dropshadow}

- Select the Forguncy file (*fgcproj) to import from and click **Open**.

![project-import-open-dialog](/assets/images/product-images/project-import-open-dialog.png)
{:.dropshadow}

- The **select Forguncy File to Import** dialog box lists all Forguncy objects such as pages, master pages, tables, server-side commands, scheduled tasks, reports, shared commands, cell style styles, list view styles, and more. Select the objects to be imported, check the data to be imported, and click **OK**.

Note: In addition, if the page or table has settings that depend on the connection information of the external database, it is necessary to select the necessary connection information of the external database and import it together. Likewise, if the page has a master page set, you must select the required master page to import along with it.
{:.note}

![project-import-select-forguncy-file-to-import-dialog](/assets/images/product-images/project-import-select-forguncy-file-to-import-dialog.png)
{:.dropshadow}

If there is a page or table with the same name in the import destination, the following dialog will be displayed.
Select suitable action to continue.

![project-import-handling-conflict](/assets/images/product-images/project-import-handling-conflict.png)
{:.dropshadow}

When you import tables, pages, master pages, server commands, scheduled tasks and reports, a folder called "Import Folder 1" is generated and the imported objects appear in this folder. Replaced objects are not included in this folder because they exist in the location where they were replaced.

![project-import-folder](/assets/images/product-images/project-import-folder.png)
{:.dropshadow}
