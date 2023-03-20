---
layout: default
title: Data Extraction and Sorting in List View
parent: List Views
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/List-views/data-extraction-and-sorting-in-list-view
nav_order: 6
---

# {{ page.title }}

There are two types of list view data extraction: extraction as preprocessing to narrow down the data to be used on the page and extraction as the act of searching for the desired data by the application user.

## Extraction as pretreatment

- Select the list view and click the list view tool (Design tab) -> Query condition.
- In the **Query Conditions** dialog, click **New Condition** to set the conditions for extracting data.

You can set multiple conditions and connect with And/Or.

You can enter the formula directly in the query condition dialog. In addition, the cell position is automatically entered by clicking the cell.

### Extraction as a Search Criteria

- Create a text box type cell for the user to enter search criteria. It is recommended to use a date type cell if the value to be searched is a date type, and use a numeric type cell if the value is a number.
- Create a button-type cell for setting the **Query** command.
- Click Commands from the right pane to open the Commands dialog and select Query from the Select Command drop-down list.
- Click the **New Condition** button to add one condition and set the conditions for the search you want to create. Here, in order to be able to search for *affiliation* by partial match, specify **affiliation** field for the field (left side) and **contains specified value** as the comparison operator.
- Specify a text box type cell for the value (right side) of the created condition. Then click the **OK** button in the **Command** dialog to close the dialog.
- Go to **Home** and click **Start** -> **Debug** to make sure the search function works.

### Sorting

By default, the list view is sorted in ascending order of the [ID] field.

- Select the list view and click the list view tool **Design** -> **Sort**.
- In the **Sort Condition** dialog box, click **New Condition** to set the condition for sorting the data.

You can also set multiple sorting criteria by clicking New Criteria.
In this case, the conditions above take precedence.




