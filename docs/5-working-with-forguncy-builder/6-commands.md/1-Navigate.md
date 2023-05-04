---
layout: default
title: Navigate
parent: Commands
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/commands/navigate
nav_order: 1
---

# {{ page.title }}

Go to another page. Even if multiple page transition commands are set in one command setting, only the first page transition command is valid. See Commands (Normal) for information on executing this command.

![navigate-command](/assets/images/product-images/navigate-command.png)
{:.dropshadow}

There are four setting methods for moving pages.

|Controls|Description|
|:--|:--|
|Pages in Forguncy|Select from the list of pages in Forguncy.|
|External page|Directly specify the address of the Forguncy application external page. Only addresses beginning with "http://" or "https://" can be specified. If you specify an address starting with "file://", you may be able to open files on network shared folders only with Internet Explorer, but that operation depends on the security settings of your web browser.|
|Cell value or formula|Specify the transition destination using a cell reference or formula. Valid values ​​are page names within the Forguncy application, or external page addresses. For example, if you have "page 2" and the page name in cell A1, you can write "=A1" <br/> ![navigate-select-value-command](/assets/images/product-images/navigate-select-value-command.png)|
|open in new tab|If this check option is checked, the transition destination page will be opened as a new tab in the web browser. If a command is also set after this command, the next command will be executed after the page transition.|

## Advanced Settings for "Pages in Forguncy"

If you select a page other than "<previous page>" and "<new page>" in [Page in Forguncy], you can configure the following detailed settings.

You can increase the setting of values ​​passed to the transition destination page with [New value] and [Delete value].

![navigate-advanced-control-command](/assets/images/product-images/navigate-advanced-control-command.png)
{:.dropshadow}

### Passing the value to the transition destination page

Passes a value to a specific cell on the transition destination page at the time of page transition.
The following methods can be used as [Value to pass].

- Fixed value
- Specify the cell of the transition source page
- Specify a cell in the list view of the transition source page
    
    *In this case, the value of the specified cell of the current record (the row where the focus exists at the time of execution) will be the [Passed value].
- Using formulas

In [Transition destination page cell], only the cell specification of the transition destination page can be set.

Note: Basically, [Value to pass] is treated as a string because the type cannot be determined. If you want to treat it as a type other than a string, use a cell reference or set it together with a formula such as "=1" or "=VALUE(1)".
{;.note}

### Delete cache of query result and sort result of transition destination page

The results of the [Query] command and [Sort] command, as well as the results of filtering and sorting by the list view header are cached in the web browser so that those results are retained when the page is returned to. increase. However, those cached results may not work as intended, such as overwriting the result of the [Query] command set in the page load command. Checking this option removes the cached results of the Query and Sort commands, as well as the results of filtering and sorting by list view headers.

### Data binding setting of transition destination page

If there is data binding on the transition destination page, set how to load the binding data. In other words, it specifies whether to pass the information of the current row of the transition source to the transition destination page, and thereby whether to read the linked data of the transition destination page.

|automatic|If the transition destination page contains a command with a process type of "Add" with "Update table data", the consolidated data will not be loaded. Otherwise, consolidation data is loaded.|
|Load Consolidated Data|Consolidated data is always loaded. It is suitable when the transition destination page is an edit page, or when a new record is added based on existing data.|
|Do not load consolidated data|Consolidated data is not loaded. Suitable when the transition destination page is a page for new registration.|

## "Cell value or formula" advanced settings

Only the following parts are different from the detailed settings of "Page settings in Forguncy" above.

![navigate-select-value-advanced-setting-command](/assets/images/product-images/navigate-select-value-advanced-setting-command.png)
{:.dropeshadow}

### Passing the value to the transition destination page

Passes a value to a specific cell on the transition destination page at the time of page transition.

The following methods can be used as [Value to pass].

- Fixed value
- Specify the cell of the transition source page
- Specify a cell in the list view of the transition source page
    * In this case, the value of the specified cell of the current record (the row where the focus exists at the time of execution) will be the [Passed value].
- Using formulas

In [Transition destination page cell name], you can assign a name to the cell that displays the passed value, and only that name can be set. 

Note: Basically, [Value to pass] is treated as a string because the type cannot be determined. If you want to treat it as a type other than a string, use a cell reference or set it together with a formula such as "=1" or "=VALUE(1)".
{:.note}

