---
layout: default
title: Show Popup
parent: Commands
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/commands/show-popup/
nav_order: 2
---

# {{ page.title }}

Displays other pages in Forguncy in a popup window. Even if multiple popup window display commands are set in one command setting, only the first popup window display command is valid. See Commands (Normal) for information on executing this command .

![command-show-popup](/assets/images/product-images/command-show-popup.png)
{:.dropshadow}

The settings for the Show Popup Page command are as follows:

## Specify target page

### Pages in Forguncy
Select from the list of pages in Forguncy.

### cell value or formula
Specify the transition destination using a cell reference or formula. Valid values ​​are page names within the Forguncy application. For example, if you have "page 2" and the page name in cell A1, you can write "=A1".

![command-transition-destination%20](/assets/images/product-images/command-transition-destination%20.png)
{:.dropshadow}

## Pop-up display mode

You can specify one of the following three methods for popup display. The default is Dialog Window.

**Dialog window**

- You can close the popup window by clicking the close button on the right side of the title bar or executing the [Close Popup Window] command.
- The close button on the right side of the title bar can be hidden by enabling [Hide close button on pop-up windows] in the application settings .
- The display position of the popup window is the center of the screen.
- The screen area other than the popup window is covered with a semi-transparent color and operations are disabled (modal display).
- You can move the popup window by dragging the title bar.
- The theme color "Accent 1" is automatically applied to the title bar color.

**Drop down**

- No title bar is displayed.
- Click outside the popup window area, execute the [Close Popup Window] command, or press the ESC key to close the popup window.
- The display position of the popup window is the center of the screen.
- A popup window is displayed at the cell position specified in [Position to display popup].

**Popup without title bar**

- No title bar is displayed.
- Click outside the popup window area, execute the [Close Popup Window] command, or press the ESC key to close the popup window.
- Screen areas other than pop-up windows are covered with a semi-transparent color.

## Display position of popup

When [Popup display mode] is "Dropdown", set the display position by specifying the cell. If this property is not set, it will be displayed adjacent to the cell where the [Display Popup Window] command was executed, but if the cell where the command was executed is a cell on the list view, it will be displayed in the center of the screen.

## Advanced Setting

The following settings can be made as advanced settings. You can set more values ​​to pass to the popup page with [New value] and [Remove value].

![command-show-popup-advanced-settings](/assets/images/product-images/command-show-popup-advanced-settings.png)
{:.dropshadow}

### Passing the value to the transition destination page

Passes a value to a specific cell on the transition destination page at the time of page transition. The following methods can be used as [Value to pass].

- Fixed value
- Specify the cell of the transition source page
- Specify a cell in the list view of the transition source page
  * In this case, the value of the specified cell of the current record (the row where the focus exists at the time of execution) will be the [Passed value].
- Using formulas

In [Transition destination page cell], only the cell specification of the transition destination page can be set.

### Delete cache of query result and sort result of transition destination page

The results of the [Query] and [Sort] commands, as well as the results of filtering and sorting by list view headers, are now cached in the web browser and retained when the page is displayed again as a popup window. has become However, those cached results may not work as intended, such as overwriting the result of the [Query] command set in the page load command. Checking this option removes the cached results of the Query and Sort commands, as well as the results of filtering and sorting by list view headers.

### Data binding setting of transition destination page

If there is data binding on the transition destination page, set how to load the binding data. In other words, it specifies whether to pass the information of the current row of the transition source to the transition destination page, and thereby whether to read the linked data of the transition destination page.

- automatic: If the transition destination page contains a command whose process type is "Add" with "Update table data", the consolidated data will not be read. Otherwise, consolidation data is loaded.
- Load Consolidated Data: Consolidated data is always loaded. It is suitable when the transition destination page is an edit page, or when a new record is added based on existing data.
- Do not load consolidated data: Consolidated data is not loaded. Suitable when the transition destination page is a page for new registration.

Note: When passing a value to the popup window, if the destination page is a list view, the rows in the list view that match the passed value will be selected in the list view of the destination page. . Values ​​in the list view are never overwritten.
{:.note}

## "Cell value or formula" advanced settings

Only the following parts are different from the detailed settings of "Page settings in Forguncy" above.

![command-select-value-advanced-settings%20](/assets/images/product-images/command-select-value-advanced-settings%20.png)
{:.dropshadow}

### Passing the value to the transition destination page

Passes a value to a specific cell on the transition destination page at the time of page transition. The following methods can be used as [Value to pass].

- Fixed value
- Specify the cell of the transition source page
- Specify a cell in the list view of the transition source page
  * In this case, the value of the specified cell of the current record (the row where the focus exists at the time of execution) will be the [Passed value].
- Using formulas

In [Transition destination page cell name], you can assign a name to the cell that displays the passed value, and only that name can be set.

