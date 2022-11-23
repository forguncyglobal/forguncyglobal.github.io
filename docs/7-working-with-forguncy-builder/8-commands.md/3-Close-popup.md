---
layout: default
title: Close Popup
parent: Commands
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/commands/Client-side-commands/close-popup
nav_order: 3
---

# {{ page.title }}

Close popup command closes the popup window that appears on its execution.

![command-close-popup](/assets/images/product-images/command-close-popup.png)
{:.dropshadow}

|Control|Description|
|:--|:--|
|Return value to parent page|If checked, returns the values ​​of the page displayed within the popup window back to the calling page.|
|Refresh the parent page's bound data|If checked, it will update the consolidated data that is bound to the parent page to the latest. <br/>If the parent page's list view's load-on-demand setting is enabled, the records dynamically loaded by load-on-demand will be displayed in the list view by updating (reloading) the binding data to the latest. can not be displayed. Therefore, if the current record existed in dynamically loaded data by load-on-demand, the current record is not retained.|
|Pass query results to parent page|If checked, pass the results of queries made in the popup window to the parent page. As a result, by executing the "query" command after the "close popup window" command, the query results can be reflected on the parent page side as well.|

The value returned by the Return value to parent page option will be the value of the cell specified in the Transition destination page cell of the Show Popup Window command. Also, the return destination will be the cell specified in [Passed value] set by the [Display popup window] command. Any cell other than these specified cells cannot be respecified with the Close Popup Window command. 
{:.note}

If the cell specified in [Value to pass] of the [Show Popup Window] command is a cell on a list view, the row in the list view that matches the returned value is selected in the list view of the transition source page. state. Values ​​in the list view are never overwritten. Note that if there are multiple [Values ​​to pass] set with the [Display popup window] command, only the last [Values ​​to pass] will be used to determine whether the above values ​​match.
{:.note}

## Hide the close (x) button on popup windows

If you click the close (x) button at the top right of the popup window screen, the settings of various check boxes of the "Close popup window" command will not be reflected. In this case, you should hide this button, create a separate "Close" button, and set the command for that button to "Close Popup Window".

To hide the (x) button above, check the "Hide pop-up close button" check box from the following screen displayed by clicking the "File" menu.

![command-close-popup-options-settings](/assets/images/product-images/command-close-popup-options-settings.png)
{:.dropshadow}