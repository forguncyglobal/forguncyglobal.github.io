---
layout: default
title: Call Stored Procedure
parent: Commands
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/commands/Client-side-commands/call-stored-procedure
nav_order: 7
---

# {{ page.title }}

By using the Call Stored Procedure command, it is possible to execute a specific stored procedure in an external database. This command supports only the following external database stored procedures.

- SQL Server
- MySQL

![command-call-stored-procedure](/assets/images/product-images/command-call-stored-procedure.png)
{:.dropshadow}

|Controls|Description|
|:--|:--|
|Connection information|Select and select the connection to the external database where the stored procedure of interest resides. If you have not yet created connection information, you can create new connection information by clicking the Open connection information dialog... hyperlink. See Managing External Database Connections for more information.|
|stored procedure name|Depending on the selected connection information, a drop-down list will appear with a list of available stored procedures. Select and configure the stored procedure you want to run. <br/> If you have changed the stored procedure or its parameters on the external database side, click the [ ] button to update the information to the latest state and then set it again.|
|Return code display cell|Specifies the cell that displays the stored procedure return code, which is an integer value. You cannot display the result set. This setting is only available for SQL Server.|
|Parameter list|When [Stored procedure name] is set, [Parameter name], [Parameter value], and [Output parameter display cell] are displayed according to the stored procedure, and if they can be set, they can be entered. <br/> Note that automatic type conversion to the format required by the stored procedure is not performed. Therefore, it is necessary to change the value to the required format before passing it.|
|role privileges|Set the role that allows execution of this stored procedure.|

Steps to execute **Call stored Procedure** are as follows-

To use this command, a stored procedure must be created in the external database to connect to. Here, the case where the following stored procedure is created in SQL Server is explained as an example.

![command-call-stored-procedure-example](/assets/images/product-images/command-call-stored-procedure-example.png)
{:.dropshadow}

- Select the connection information for the external database where the stored procedure to call resides and set the stored procedure name.

![command-call-stored-procedure-](/assets/images/product-images/)

- Set the [Parameter value] and [Output parameter display cell] displayed in [Parameter list] as follows.

![command-call-stored-procedure-](/assets/images/product-images/)

- Click the Start Debugging button on the Home ribbon tab to see your application in action. <br/> Enter an arbitrary number in the parameter value input box and click the "Execute" button to execute the target stored procedure, update the data in the table, and check that the returned output parameter is displayed in the target cell. I can confirm.

![command-call-stored-procedure-](/assets/images/product-images/)

Note: <br/><br/> In the case of MySQL, even if the stored procedure is changed on the MySQL side, the change will not be reflected by the cache. You will need to restart Forguncy Builder for the changes to take effect. <br/><br/>If you change the stored procedure on the external database side, you will need to republish the Forguncy application (without checking the "Change database on server" check option). <br/><br/>After executing the "Call Stored Procedure" command, all list view and data bound cells and cell types on the page will be reloaded regardless of whether the database is the target database of the stored procedure.
{:.note}