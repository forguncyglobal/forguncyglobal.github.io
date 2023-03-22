---
layout: default
title: Project
parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Project/
nav_order: 1
has_children: true
has_toc: true
---

# {{ page.title }}

A project represents a unit that contains created application as a file. This section explains various project operations such as *Create*, *Open*, *Save*, and *Import*. 

### Create
You can create project from a excel sheet, access database, or a template. Forguncy allows several formats to save a project. You can import table and page data from another project file (FGCP file) into another. 

### Save
Forguncy has several project formats. Read [Save Project](# ) for more details.

### Open
Forguncy has several project formats. You can open projects created in older versions. Do this will convert the project into new version and you will not be able to convert it back to its original format. Read [Loading Projects](# ) for more details.

### Import
You can import table and page data from another project file (FGCP file) into the open project file. Read [Importing data from other projects](# ) for more details.

## Project Format

Forguncy projects are saved in *.fgcpproj format. 
This is the save format of Forguncy Builder Project. All the information required to create an application is included in a single project file.
It is a project format in which multiple files necessary for creating an application are stored together in one folder.

## Creating a New Project

Steps to create a new project are-

- Open Forguncy Builder and click **New**. If Forguncy Builder is already open then go to **File** and click **New**.
- Select **Blank**.

![project-new-project](/assets/images/product-images/project-new-project.png)
{:.dropshadow}

- A new project screen will appear.

![project-new-project-screen](/assets/images/product-images/project-new-project-screen.png)
{:.dropshadow}

## Saving a Project

Steps to save a project are-

- Go to **File** and click **New**.
- Select **Save** to save current project with the exsisting name and **Save as** to save with a new name.

![project-new-save](/assets/images/product-images/project-new-save.png)
{:.dropshadow}

![project-new-save-as](/assets/images/product-images/project-new-save-as.png)
{:.dropshadow}

- If you click **Save As**, specify a file name. The extension of the file will be *.fgcpproj.

![project-new-save-as-dialog](/assets/images/product-images/project-new-save-as-dialog.png)
{:.dropshadow}

 Files and images uploaded by debugging during development are saved in a folder that is automatically generated in the same folder as the project file.

## Saving a Project Summary

Allows you to export the current project summary to microsoft Excel document.

![save-project-summary](/assets/images/product-images/save-project-summary.png)
{:.dropshadow}

Choose the location and enter file name as required. 
![save-project-summary-export](/assets/images/product-images/save-project-summary-export.png)
{:.dropshadow}

Note: File type can only be XLSX (*.xlxs) i.e. **Save as type** is not editable.
{:.note}







