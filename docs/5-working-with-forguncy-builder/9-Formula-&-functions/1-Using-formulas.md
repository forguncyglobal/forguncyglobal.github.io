---
layout: default
title: Using Formulas
parent: Formulas & Functions
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Formulas-&-functions/using-formulas/
nav_order: 1
---

# {{ page.title }}

Formulas can be set in cells and in list view template rows just like in Excel.

Formulas can be typed directly into the cell or set as the cell's default value, depending on the cell type. The following cell types are supported when setting as the default value for a cell

- Text box
- Multiline text box
- Checkbox group
- Radio group
- Combo box
- Numerical value
- Date
- Times of Day
- User selection combo box

You can also type directly into the cell by entering the formula followed by "=". Let's take an example of adding two values.

![formula-enter-in-cell](/assets/images/product-images/formula-enter-in-cell.png)
{:.dropshadow}

Go to **Home** tab and click on the **Start** to debug. You will see the results of formula applied in a cell as:

![formula-enter-in-cell-output](/assets/images/product-images/formula-enter-in-cell-output.png)
{:.dropshadow}

Note: In Forguncy, formulas are not calculated unless you run the application (unlike in excel). 
{:.note}

## Relative Cell References in Listview

The results of calculations that refer to cells within a list view may sometimes vary depending on whether they are displayed within the list view or outside the list view.

![formula-relative-cell-references-in-listview](/assets/images/product-images/formula-relative-cell-references-in-listview.png)
{:.dropshadow}

Formula applied within a row template is applicable only for the listview's respective row (even if you specify the range of rows below the row template or the entire list view). Hence, data validation and functions like VLOOKUP that require column-wise cell range references in commands are effectively unusable. You can avoid such problems by setting formulas that use the VLOOKUP function in normal cells and referencing the results from data validation rules and commands.

## Absolute Cell References in Listview

Cell reference in listviews works differently by using absolute cell reference than relative cell reference. 

![formula-absolute-cell-references-in-listview](/assets/images/product-images/formula-absolute-cell-references-in-listview.png)
{:.dropshadow}

On making an absolute reference to cell E5 with "=$E$5" in cell R5, at runtime all cells of column R will have the value  equals to the first row of the "Item" column.

<!--

## Precedence of Formulas, Data Binding, and User Input

A single cell can have both formulas and data bindings. Formulas can also be set for cells that allow user input, such as textbox cell type. 

In such cases, the value read by the data binding, the value determined by the formula calculation, and the value entered by the user applies:

- If data binding loads data into that cell, the value loaded with data binding takes precedence. However, even if data binding is set, the calculation result of the formula is applied when the data is not read like the new input page.

- Regardless of whether the data is loaded by data binding or not, if the data referenced by the formula is changed, the formula will be recalculated, so the calculation result of the formula will be applied.

- If the user enters a value in a cell such as a textbox cell type, the entered value is applied. Again, if a subsequent recalculation of the formula occurs, the value entered by the user will be overwritten by the result of the formula calculation.

**For Excel export**

If there is data loading by data binding at the time of displaying the target page, the value displayed on the screen will be exported as it is regardless of the subsequent operation.

If there is no data loaded by data binding when the target page is displayed, the preset formula will be exported regardless of subsequent actions.

**For PDF export**

If there is data loading by data binding at the time of displaying the target page, the value displayed on the screen will be exported as it is regardless of the subsequent operation.

If data is not read by data binding at the time the target page is displayed, the calculation result of the preset formula will be exported regardless of subsequent operations.

 -->