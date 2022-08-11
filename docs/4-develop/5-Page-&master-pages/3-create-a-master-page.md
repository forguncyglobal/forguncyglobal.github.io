---
layout: default
title: Create A Master Page
parent: Page &amp; Master Pages
grand_parent: Develop
permalink: /develop/Page-&-master-pages/create-a-master-page/
nav_order: 3
---

# {{ page.title }}

Use master pages to give your application a uniform look and to organize similarly formatted pages. 

When you apply a master page to a page, that page appears as a child page in a placeholder area within the master page.

A page with a master page applied will have an icon to the right of the page name in the navigation window .

Note: You can create master pages for mobile devices. Mobile master pages can only be applied to mobile pages. The creation method and operation are the same as for a normal master page. A mark appears in the navigation window.
{:.note}

Note: If the size of the child page is larger than the size of the placeholder on the master page, how the child page is displayed depends on how it is displayed on the master page in the child page's Page Setup pane. It depends on your settings. See Applying Master Pages for more information.
{:.note}

Steps to create a new master page:
- Click Create ribbon tab - Master Page.
- Select a template for the master page in the Select Template dialog. The first template is a top banner and vertical menu, the second template is a top banner and horizontal menu, and the third template is a blank template. Templates 1 and 2 are affected by theme changes. After selecting a template, click the OK button to create a new master page.
- Edit the master page.

Note: You can also duplicate an existing master page to create a new master page.
{:.note}

##### Resizing
Resize to change the size of the placeholder:
- Select the placeholder to be resized and click Placeholder Tool [Design] > [Start resizing].
- Drag the corners to resize.
- Click [Placeholder Tools] > [Finish Resize]. When you apply the master page, the child pages show dotted lines in the areas that can be displayed for placeholders.

Note: If the child page does not fit in the placeholder, you can select one of the following three display methods in "How to display on the master page" in the page settings of the child page: overflow, scroll, cut
{:.note}

##### Page Setup For Master Pages
After selecting and opening the master page you want to edit from the navigation window, click the [Page Settings] tab at the bottom of the right pane to configure settings.

|name|Sets the name of the master page.|
|Number of lines|Sets the number of lines on the page.|
|number of columns|Sets the number of columns on the page.|
|Page stretch mode|The page will stretch or shrink depending on the browser at runtime. For more information, see Page Stretch|

## Create A New Mobile Master Page
- Click Create ribbon tab - Mobile Master Page.
- Select a template for the master page in the Select Template dialog. The first template is a top banner and bottom menu, the second template is a blank template. The first template is affected by theme changes.
- Edit the mobile master page.
    Note: You can also clone an existing mobile master page to create a new mobile master page.
    Right-click the master page in the Navigation Pane and select Duplicate.
    {:.note}

##### Resize Placeholder
Child mobile pages appear in placeholders on the master mobile page.
If you want to change the size of this placeholder, perform a resize.
- Select the placeholder to be resized and click Placeholder Tool [Design] > [Start resizing]. A blue line surrounds the placeholder.
- Drag the corners to resize.
- Click [Placeholder Tools] > [Finish Resize].

##### Apply Master Mobile Page Created To Mobile Page
- Specify the master page name you want to apply in the page settings of the mobile page.
- On the mobile page, the area that can be displayed for the placeholder is indicated by a dotted line. If you specify a mobile master page, the mobile page will show dotted lines in the areas that can be displayed for placeholders.

Note: If the child page does not fit in the placeholder, you can select one of the following three display methods in "How to display on the master page" in the page settings of the child page.
{:.note}
- overflow
- scroll
- cut
{:.note}

##### Mobile Master Page Page Setup
After selecting and opening the mobile master page from the navigation window, click the [Page Setup] tab at the bottom of the right pane to configure settings

|Name|Sets the name of the mobile master page.|
|Number of lines|Sets the number of lines on the page.|
|Number of columns|Sets the number of columns on the page.|
|Page stretch mode|The page will stretch or shrink depending on the browser at runtime. <br/>For more information, see Page stretching.|

## About Built-in Master Pages
When you create a new project in Forguncy, one master page is already prepared.
You can customize and use this master page.

Note: Names cannot be changed or deleted.
{:.note}

After selecting and opening the built-in master page you want to edit from the navigation window, click the [Page Settings] tab at the bottom of the right pane to configure settings.

|Number of lines|Sets the number of lines on the page.|
|Number of columns|Sets the number of columns on the page.|
|Page reset|Returns the built-in master page being edited to its default state.|
|Page stretch mode|The page will stretch or shrink depending on the browser at runtime.
For more information, see Page Stretch.|

## Applying Master Pages
You can use master pages to give your pages a consistent look, titles, and common menu items.
This section describes how to apply a master page to your pages.

Note: You can create a master page for mobile devices and apply it to your mobile pages. Mobile master pages can only be applied to mobile pages. The application method is the same as for a normal master page.
{:.note}

- Right-click the page to apply the master page in the navigation window → [Master Page Settings] → click the name of the master page to apply. When a master page is applied, a mark will appear next to the page name in the Navigation Pane. When a mobile master page is applied, a mark will appear next to the page name in the navigation pane.

##### Applied Master Page Page Settings
Set the applied master page in the "Page Setup" pane.
This section describes settings related to master pages.

##### How to display the master page
Set the processing when the child page cannot be displayed in the placeholder of the master page.

|Overflow|The placeholder expands to fit the size of the child page to show all content.|
|Scroll|A scroll bar appears. * This setting is effective only in the horizontal direction.|
|Cut|The child page is displayed to the size of the placeholder (the protruding part is cut off). * This setting is effective only in the horizontal direction.|



