---
layout: default
title: Process Bar
parent: Cell Types
grand_parent: Develop
permalink: /develop/Cell-types/Process-bar/
nav_order: 20
---

# {{ page.title }}

The Process Bar automatically displays corresponding buttons, workflow states, assignees, etc. for the created [Workflows](https://docs.forguncy.net/develop/Workflows/). The user can proceed with the workflow (approval/ rejection)process by operating the buttons displayed on the Process Bar..

Note: This cell type cannot be set in the row template area of ​​a list view.
{:.note}

Steps to create a Process Bar with cell type:

- Select a cell range and go to **Cell Type** drop-down list. 
- Select **Process Bar** cell type. 

![process-bar-cell-type](/assets/images/product-images/process-bar-cell-type.png)
{:.dropshadow}

Note: Make sure the Process Bar has enough space to display workflow states, buttons, etc.
{:.note}

- Configure the Process Bar settings in the **Cell Type** tab of right pane. The **Preview** combo box displays the status specified in the [Workflows](https://docs.forguncy.net/develop/Workflows/) settings . 
- Select from here to see how the Process Bar will appear on the screen when in that state.

![process-bar-preview-settings](/assets/images/product-images/process-bar-preview-settings.gif)
{:.dropshadow}

The controls are:

|Table name|Specify the table associated with the workflow bar. Only tables with workflow enabled are displayed in dropdown.|
|Show creation info of the record|Displays information such as the person in charge who created the record with the date and time.|
|Show modification info of the record|Displays information such as the person who last updated the record, the date and time, etc.|
|Show the current assignees|Shows the assignee currently designated in the workflow.|
|Show the current state info|View the current state of the workflow.|
|Show history popup when the current state info is clicked|Pops up the workflow change history.|
|Show action button|Shows Submit, Approve, Reject buttons depending upon the state of the workflow.|
|Preview|Allows you to preview each workflow state.|
|Allow editing comments when changing workflow state|Allows editing of comments when changing the state of a workflow (pressing the change state button).|
|Edit Action Button Style...|To adjust the appearance of the button as needed. You can set common styles or individual styles. Individual styles take precedence over common styles.|

![process-bar-edit-action-button-style](/assets/images/product-images/process-bar-edit-action-button-style.png)
{:.dropshadow}

The **Edit Action Button Style** dialoge allows:
- **Common Style**: You can define styles that are commonly used for all action buttons. Click **Settings** button to set layout, font, color, border, etc. in the **Common Styles** dialog box.

![process-bar-common-style](/assets/images/product-images/process-bar-common-style.png)
{:.dropshadow}

- **Single Style**: You can define the styles used by buttons for specific actions. Select an action button from the combobox, click the **Add** button, then click **Settings**. Set the layout, fonts, colors, borders, etc. in the **Common Styles** dialog box. Click **delete** to delete an individual style that you have set.

Note: <br/> You cannot change the style of the Administrator's Change Assignee action button. <br/> You cannot change the style of action buttons on mobile.
{:.note}