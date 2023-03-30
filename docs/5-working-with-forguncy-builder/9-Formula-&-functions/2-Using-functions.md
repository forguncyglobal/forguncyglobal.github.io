---
layout: default
title: Using Functions
parent: Formulas & Functions
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Formulas-&-functions/using-functions/
nav_order: 2
---

# {{ page.title }}

Functions can be used in formulas in cells, just like in Excel. Forguncy supports over 300 functions. Such as VLOOKUP function which can automatically display the value corrosponding to the ID.

There are two methods of using functions in Forguncy:

- Enter directly in the formula bar.

![function-formula-bar](/assets/images/product-images/function-formula-bar.png)
{:.dropshadow}

Type '=' followed by the first letter of a function name in the formula bar to display a list of matching function names. Selecting a function name with the cursor key displays the outline of that function.

- Select from **Formula** -> **Functions**.

![functions-formula-tab](/assets/images/product-images/functions-formula-tab.png)
{:.dropshadow}

![insert-function-dialog](/assets/images/product-images/insert-function-dialog.png)
{:.dropshadow}

Note: You can also open the dialog box by clicking **fx** icon to the left of the formula bar.

Double-click the function for the selection. Here, is an example showing average of two numbers:

![functions-example](/assets/images/product-images/functions-example.png)
{:.dropshadow}

To specify the list view part outside the list view, just specify a single cell of the row template, unlike the specification method in Excel. 

For example: In Excel =MATCH(10,A1:A5,0) is used but in Forguncy the function is defined as =MATCH(10,A2,0).

![function-match-argument](/assets/images/product-images/function-match-argument.png)
{:.dropshadow}