---
layout: default
title: Hyperlinks
parent: Cell Types
grand_parent: Develop
permalink: /develop/Cell-types/hyperlinks/
nav_order: 9
---

# {{ page.title }}

This cell type allows you to create a hyperlink.

![hyperlink_celltype](/assets/images/product-images/hyperlink_celltype.png)
{:.dropshadow}

Steps to create a Hyperlink cell type:

- Select a cell, and go to the **Cell Type** drop-down list. 
- Select **Hyperlink** cell type. 
- The selected cell content will become a Hyperlink type.
- Go to the **Cell Type** tab at the bottom of the right pane to configure hyperlink settings. 

![hyperlink_celltype_settings](/assets/images/product-images/hyperlink_celltype_settings.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|Commands..|Sets the command to be executed when the display text is clicked.|
|Set UI Permissions..|Show/hide and enable/disable the cell type for respective role. <br/> Note: This control has limitations in the list view.|
|Text To Display|Specifies the text displayed as a hyperlink.|
|Click Area|Select the hyperlink click area as *Text Only* or *Entire Cell*. This item cannot be set in the cell type on the list view.|
|Disabled|Disables user interaction with the hyperlink and renders it unusable. <br/> Note: This control has limitations in the list view.|
|Hide|Make the hyperlink invisible. <br/> Note: This control has limitations in the list view.|

- Data concatenation is performed as necessary.

Note: Hyperlink type cells are not a user interface for users to enter/edit values, so there are not many opportunities for data binding, but it is possible to display table data as hyperlink text using data binding.
{:.note}