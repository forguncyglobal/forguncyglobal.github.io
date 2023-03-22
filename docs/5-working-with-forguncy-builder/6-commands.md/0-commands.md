---
layout: default
title: Commands
parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/commands/
nav_order: 6
has_children: true
has_toc: true
---

# {{ page.title }}

The command is used to perform some processing based on the user's action, such as switching pages when a button is pressed, extracting and displaying some specific data, etc. Commands can be set for specific cell types, pages, workflows, etc. Multiple commands can be configured on the command setting screen. Those commands will be executed in order of their configuration.

## Command Execution

The command execution time differs depending on the cell type for which the command is set-

### Command to be executed on click

If you set a command for cell types- Buttons, hyperlinks, images, image objects, background image objects, the command will be executed when these cell types are clicked.

### Command to be executed when the value changes

If you set a command for cell types- Text Box, Multiline Text Box, Check Box, Check Box Group, Radio Group, Combo Box, Number, Date, User Select Combo Box, Phonetic Text Box, the command will be executed when the value change is confirmed. 

The confirmation timing of changes in the cell type differs depending on the cell type and does not necessarily match with the change timing intended by the application user. 

*For example*, in the case of a text box type cell, simply entering a string in the text box does not commit the change, infact the change happens when the focus leaves the text box.

- Changes to values ​​that are conditions for executing **Commands to be executed when values ​​are changed** are not limited to changes made by users. 
- Any value change after the page has finished loading, such as formulas, data bindings, cell property set commands, JavaScript APIs, etc. will execute the command.
- Even if you change the value twice or more in a row using the JavaScript API or the cell property setting command, the **Command to be executed when the value changes** is executed only once.
{:.note}

### Commands to be executed on page load
If you set a command from Command on Page Load via **Page Setup** tab in the right pane, that command will be executed when the page loads.

### Command to be executed on double-clicking a ListView

If you select the entire list view area and set a command from **Double click commands...** in the **Cell Type** tab in the right pane, that command will be executed when the list view area is double-clicked. 

The double-click target area does not include corner headers, column headers, and scrollbars.

Note: If the **Allow Editing Listview** option is enabled, the command to be executed on double-click will not work.
{:.note}

The most common usage scenario is when you want to display a list view on a popup window and double-click to select a row and close the popup window at the same time. In such cases, set the Close Popup Window command as the command that executes when you double-click the list view.

### Commands that run before and after workflow actions
If you set a command from the **Command** buttons on the left and right of **Action** in the Workflow dialog, that command will be executed when the workflow button is clicked.


The command processing may fail due to external factors, and subsequent commands will not be executed in the event of failure.

Note: In addition to the commands listed here, you can include more commands by adding plugins.
{:.note}


## Command setting method
By setting commands, you can specify actions that your application performs after a user presses a button or a page loads.

For the cell type, click [Command] on the [Cell Type] tab in the right pane to display the [Command] dialog shown below. When loading a page, click [Edit Commands When Loading Page] on the [Page Settings] tab in the right pane to display the [Command] dialog shown below.

![command_window](/assets/images/product-images/command_window.png)
{:.dropshadow}

Click Select Command to select the command to run. Refer to the following for the contents of the command.

![command_list](/assets/images/product-images/command_list.png)
{:.dropshadow}

Set command details. Details vary for each command. (Example: For updating table data)

![command_update_data_table](/assets/images/product-images/command_update_data_table.png)
{:.dropshadow}

- You can run multiple commands for a single cell type by clicking New Command. 
- Click [Delete Command] to delete the selected command.
- Click [ ] or [ ] to change the command execution order.
- Commands are displayed in a hierarchical structure on the left side of the screen, making it easy to understand what kind of processing is set. Also, each command can be moved by dragging and dropping.
- Right-clicking a command displays a pop-up menu that allows you to perform the following command operations.

![command-blank_popup-menu](/assets/images/product-images/command-blank_popup-menu.png)
{:.dropshadow}

|Insert|The command will be added after the selected command.|
|Duplication|Creates a duplicate of the selected command.
|Delete|Deletes the selected command.|
|Invalidation|Disables the selected command and prevents it from running. A strikethrough appears above the command when the command is disabled. However, conditional branch commands cannot be disabled.|
|Undisable|Undisables a disabled command so that it can be executed. Once disabled, the strikethrough will no longer be displayed.|
|Move up|Moves the command execution position up one to change the execution order.|
|Move down one|Moves the command execution position down one position to change the execution order.|

Right-clicking a blank area of ​​a command displays a pop-up menu that allows you to perform the following command operations.

|Add new command|Select the command to add it as a new command.|
|Expand all commands|Expands all configured commands.|
|Collapse all commands|Collapses all configured commands.|
|Converting to reusable commands|Converts the configured set of commands into reusable commands.|

You can enter the contents of the command in "Comment".

If you want to set similar command settings to other cells, you can copy and paste only the command settings while keeping the cell type and format as they are.

![command-copy-command](/assets/images/product-images/command-copy-command.png)
{:.dropshadow}

- Select the cell where you want to copy the command and click the Copy button on the Home ribbon tab (or press Ctrl + C).
- Select the destination cell, expand the Paste dropdown button on the Home ribbon tab, and select Command.

FYI: Copying a command from a normal cell to a list view or from a list view cell to a normal cell is invalid. Also, if you use [Undo] or [Redo] for the copy operation of the command, the result may not be correct.
{:.note}