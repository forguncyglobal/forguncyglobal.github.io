---
layout: default
title: Update Data Table
parent: Commands
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/commands/update-data-table
nav_order: 4
---

# {{ page.title }}

This command allows updating, adding, and deleting field values ​​in a table that are data bound to page cells. You can operate on a single table or multiple tables at once depending upon the requirement. 

Even if the field is not bound to data, you can update or add data by specifying Non-data bound field with this command. The delete process deletes the entire record regardless of data binding settings.

Note: To update the data in the list view, please use the **Operate Listview** command.
{:.Note}

<!-- The default found set is the current record unless you change the Record to update in advanced settings. The current record is the record selected in the list view. Even if there is no list view on the page, if any record is selected in the list view of the transition source page, it becomes the current record. For details, please refer to "Role of list view" in What is list view? -->

If you have set a data input rule for any cell on the page, the validation process for that input rule will be performed when this command is executed. If the validation process does not pass, the table data will not be updated. 

<!-- Refer Cell Data Validation Rules for the details. -->

## To update Single Table

The image below shows the screen for updating, adding, and deleting a single table. Refer below screenshot for the field selection. 

![command-update-data-table](/assets/images/product-images/command-update-data-table.png)
{:.dropshadow}

Click **Enable transaction processing** to operate with the records of multiple tables at once by executing a single command.

## To update Multiple Tables

The image below shows a screen for updating, adding, and deleting multiple tables with a single command.
If for some reason one of the operations fails during execution, you can roll back all the operations registered within this command. 

If you execute the **Update Data Table** command multiple times and the process fails for some reason, you can roll back only the table specified in that command. 

If you want to manage multiple table operations in a transaction, specify them in one **Update Data Table** command.

Note: The rollback will work correctly even if the database types are mixed such as SQL Server tables mixed with Forguncy's internal database tables.
{:.note}

Click the switch screen button to work with the records of a single table. Here, you can

- Increase the number of tables to be updated.
- Reduce the number of tables to be updated.
- Move the order of the tables to be updated.

![command-update_data_table-multiple-tables](/assets/images/product-images/command_update_data_table-multiple-tables.png)
{:.dropshadow}

|Controls| Description|
|:--|:--|
|Operation|Choose from Edit, Add or Delete depending on the type of processing you want.|
|Table|Select the table you want to update|
|Other Unbind Columns|You can define values for respective columns here if the updated value is a fixed value or a value that does not exist on the page, apart from the value entered by the user (such as using the current date and time as the updated value to register the date and time when the data was updated)|
|Row to update|Specifies the record whose data is to be updated. <br/><br/> **Current Row**-If you select the current row, the record selected in the list view will be updated. Even if there is no list view on the page, if any record is selected in the list view of the transition source page, it will be updated as the current record. <br/><br/> **Specific Row**-Selecting a specific record will allow you to specify a "new condition". All records matching this condition will be included in the update. You can update the record by selecting this, such as when you want to reflect the value entered in the non-data-bound field in the record. <br/><br/> **Selected Rows of Listview**-Updates all records in rows that are selected by clicking the row header or by selecting the row selection checkbox in the list view.|
|Show Confirmation Dialog|Displays a confirmation dialog when updating a record. You can specify a string to display in the dialog. <br/> ![command-update-data-table-show-confirm-dialog](/assets/images/product-images/command-update-data-table-show-confirm-dialog.png) <br/><br/> Note: While using Microsoft Edge, do not check the confirmation dialog saying *Hide messages from this page*. Doing so will not display the confirmation dialog of Forguncy, and Edit, Add, and Delete operations can not be performed. In case you check the Microsoft edge confirmation message and click *OK*, kindly restart the browser. <br/><br/> ![command-update-data-table-message-box](/assets/images/product-images/command-update-data-table-message-box.png) <br/> Alternatively, instead of using this confirmation dialog, you can use the conditional branch command confirmation dialog as shown in the above image to execute the update table data command. <br/><br/> In this case, the Microsoft Edge *Hide messages from this page* will not be displayed and hence, the user will not accidentally check it and need to restart the browser.|
