---
layout: default
title: Content Container
parent: Cell Types
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Cell-types/Content-container/
nav_order: 23
---

# {{ page.title }}

This cell type allows you to create a container where another page can be used as a subpage that exists in the parent page (similar to the master page displaying another normal page)

![content_container_celltype](/assets/images/product-images/content_container_celltype.png)
{:.dropshadow}

To refer to a parent page cell within a subpage of a container, name the cell as *=Page1!name* instead of using a cell reference formula as *=Page1!A1*. 

If the subpage and the parent page have different access rights i.e., if the parent page allowes access to everyone, and the child page allowes access only to administrators, a login is required to access the parent page as well. The entire page moves to the login page. After logging in, the parent page is displayed.

When exporting a page to Excel or PDF, the content of sub pages displayed within container type cells is not exported then only the sub page name is shown. If the button that invokes the export command is on a sub page (inside a container type cell) then only that sub page will be exported.

<!-- The current line of the parent page and sub page will be the same. In other words, when the user changes the current row of the subpage's list view, the associated data-bound cells on the parent page reload with the new current row.

When a button in a subpage is clicked and a "page transition" command is executed, the entire page changes, not just the subpage part.

Circular page references are not allowed.
For example, say you have page 1 and page 2, both with tab controls. On page 1, subpages set page 2 and on page 2 subpages cannot set page 1. -->

Steps to create a Content Container cell type:

- Select cells, merge, and go to the **Cell Type** drop-down list. 
- Select **Content Container** cell type. 
- The selected cell becomes content container type.
- Adjust the selection range according to the size of the subpage.
- Create a subpage for display in a container. Right-click the **Pages** and select **Create New Page**.
- Go to the **Cell Type** tab at the bottom of the right pane for the configuration.

You can do the following settings from here:

![content_container_celltype_settings](/assets/images/product-images/content_container_celltype_settings.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|Sub page|Select the subpage you want to insert. <br/> Built-in page and built-in mobile page cannot be selected. Also, you cannot select a mobile page as a subpage of a regular page or a regular page as a subpage of a mobile page.|
|Sub Page Overflow Mode|Set the display method when the subpage cannot be displayed in the container. <br/> - Overflow: The container expands to fit the size of the Sub page to show all of its contents. <br/>- Scroll: A scrollbar appears in the container. <br/>- Cut: Sub page is displayed as much as the size of the container (protruding parts are cut).|

### Switch subpages
You can switch subpages by setting the page name with the **Set Cell Property** command.