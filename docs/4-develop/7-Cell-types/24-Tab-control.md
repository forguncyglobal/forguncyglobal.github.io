---
layout: default
title: Tab Control
parent: Cell Types
grand_parent: Develop
permalink: /develop/Cell-types/tab-control/
nav_order: 24
---

# {{ page.title }}

Another page can be used as a subpage within a Tab Control cell type that exists in the parent page, just like a master page can display another normal page.
The tab title uses the title of the subpage. If no title is set, the page name will be used.

Steps to create Tab Control cell type:

- Select the area to display the subpage within the parent page.
- Go to **Home**-> **Cell Type** drop-down list and select **Tab Control** cell type.

![tab_control_celltype_creation](/assets/images/product-images/tab_control_celltype_creation.png)
{:.dropshadow}

- Create a subpage for display in a tab control. For this right-click the **Pages** tab and select **Create New Page**. Add listview and bind with a data table. Refer below screenshots as an example:

![tab_control_celltype_subpage1](/assets/images/product-images/tab_control_celltype_subpage1.png)
{:.dropshadow} 
![tab_control_celltype_subpage2](/assets/images/product-images/tab_control_celltype_subpage2.png)
{:.dropshadow}

- Adjust the selection range according to the size of the subpage
- Go to right pane->**Cell Type** tab for the settings.

![tab_control_celltype](/assets/images/product-images/tab_control_celltype.png)
{:.dropshadow}

|Control|Description|
|:--| :--|
|Tabs|Select the subpage you want to insert. You can add tabs with "+" and delete tabs with "-". You can not select Built-in pages and built-in mobile pages. Also, you cannot select a mobile page as a subpage of a regular page or a regular page as a subpage of a mobile page.|
|Active Tab Index|Sets the default tab selection. Tabs starts from 1. If the number you enter is greater than the number of tabs, the first tab will be selected.|
|Sub Page Overflow Mode|Sets the display method when the subpage cannot be displayed within the selected area. <br/> -scroll:A scrollbar appears in the tab control. <br/> -cut:Protruding parts of child pages are cut). <br/> -overflow: The area of ​​the tab control expands to fit the size of the child pages to show all the contents. Note that the Tab Control cell type borders (not cell borders) will be overridden by the expanded child pages.|
|Style Settings..|Sets the color of tab borders and tab headers. The default style of the tab header is the style of the cell.|

## Points to note when writing query commands in **Edit Pageload Commands..**

It is recommended not to describe the query command for **the same table** in the **Edit Pageload Commands..** of each sub-page. So, if you want to write a query command for same table, right-click each listview and specify query from **Data Queries**. 

![tab_control_celltype_datatable](/assets/images/product-images/tab_control_celltype_datatable.png)
{:.dropshadow}

![tab_control_celltype_dataquery](/assets/images/product-images/tab_control_celltype_dataquery.png)
{:.dropshadow}

By doing this, you can extract data with specified conditions and display it in the list view. There is no problem if the table is different when describing the query command in **Edit Pageload Commands..**, but in the case of same table, all subpages are generated when the tab control is displayed. Due to which, only the initial (first subpage) query will work. Queries listed on other subpages will not be executed because the same table has already been queried.

#### Example:

You have *2019* and *2018* tabs in your tab control and you want to display them in a listview placed on each subpage. In the listview of the *2019* tab page, the data of *2019* is extracted from *Table 1* and displayed. Similarly, in the list view of the *2018* tab, the data of *2018* is extracted from *Table 1* and displayed.

By right-clicking each list view and specifying a query with a year condition from **Data Queries**, you can extract and display the required data in that list view. If you write a query with a year condition in the **Edit Pageload Commands..** of each page, only the query for the first page of the *2019* tab will be executed, and the records extracted as 2019 will be *2019*. This will display the results appearing in the list view on both the Years tab.

## Notes on the Current Record

Even if you right-click the subpage list view and write **Data Queries**, the current record for the same table is not held on each subpage.

**If the parent page also has a list view linked to the same table** 
The current record will be the same for the parent page and the subpage. When the parent page's current record changes, the data-bound cells in each subpage changes as per the value of the parent page's current record.

**If there are multiple subpages with list views linked to the same table**
when the current record of any subpage changes, the current record of subpages will also change accordingly. For this reason, if there is a cell that is data-linked with a field of the same table somewhere in the subpage, the value of the list view of the displayed subpage will not necessarily be displayed in the cell. Displays the value of the current record.

Note: Due to the current record constraint above, the values ​​in the list view on the same page as the data bound cell will not necessarily be displayed as is in the data bound cell. To display the same table value in a cell without being caught by the current record, please use the ODATA function such as "=ODATA(~)".
{:.note}