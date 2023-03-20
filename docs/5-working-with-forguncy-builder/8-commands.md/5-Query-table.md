---
layout: default
title: Query Table
parent: Commands
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/commands/Client-side-commands/query-table
nav_order: 5
---

# {{ page.title }}

You can set conditions and extract values ​​for the specified table fields.
The extracted values ​​are reflected in the list view that is data bound with that table.

Specify table to be queried in **Data Table** field.

Click **New Condition** to set the condition. You can set multiple conditions and connect them with *And/Or*.

![command-query-table](/assets/images/product-images/command-query-table.png)
{:.dropshadow}



![command-query-table-new-condition](/assets/images/product-images/command-query-table-new-condition.png)
{:.dropshadow}

|Control|Description|
|:--|:--|
|**And/or**|The subsequent conditions can be connected to the previous condition with *And/Or*.|
|**Brackets**|Conditional expressions can be enclosed in parentheses. <br/> Select parentheses around the conditional expression. <br/> You can specify up to quadruple brackets. <br/> Parentheses can be used to set complex conditions such as "((A and B) or C) and B".|
|**Column**|Select the fields to be queried. <br/> You can also select fields that are automatically created such as *CreatedBy*, *CreationDate*, *LastModifiedBy*, *LastModificationdate*. <br/> ![command-query-table-new-condition-column](/assets/images/product-images/command-query-table-new-condition-column.png) <br/> When using related fields, the table relationships must be between tables in the same database and within the same instance. For example, the related field cannot be used <br/> -When relating between Forguncy's internal database and an external database such as SQL Server or Oracle Database. <br/> -When the instances of SQL Servers are different and the instances are not the same.|
|**Operator**|Select a condition such as *equal* or *greater than* to compare the **Column** and **Value**. ![command-query-table-new-condition-operator](/assets/images/product-images/command-query-table-new-condition-operator.png)|
|**Value**|Sets the value to compare. You can enter an expression, a value, or select a special keyword (such as %CurrentUser.UserName%). <br/>In the **Command Window** you can enter values ​​and specify cells. ![command-query-table-new-condition-value](/assets/images/product-images/command-query-table-new-condition-value.png)|

Use **Delete Condition** to remove the selected condition.