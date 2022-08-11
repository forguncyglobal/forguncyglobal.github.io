---
layout: default
title: Create A Mobile Page
parent: Page &amp; Master Pages
grand_parent: Develop
permalink: /develop/Page-&-master-pages/create-a-mobile-page/
nav_order: 2
---

# {{ page.title }}

Mobile pages can be designated as mobile versions of normal pages. In other words, when the page is accessed from a computer, the normal page is displayed, and when the page is accessed from a mobile device, the specified mobile page is automatically displayed.

Note: On mobile devices, you can delete list view data, but you cannot edit or add to it.
{:.note}

Difference between normal page and mobile page

|Page layout|Mobile pages are narrower than regular pages.|
|navigation window|Mobile pages are indicated by a different icon than regular pages.|
|cell type|I cannot set the cell type of the phonetic text box. The setting value in "Cell type" on the right pane is different from usual.|
|Page settings (settings in the right pane)|"Focus movement order" cannot be set. The mobile page to be displayed when accessing this page from a mobile device, which is set on a normal page, cannot be set on a mobile page.|
|list view|"Allow editing", "Allow adding new lines", "Allow autofill" and "Allow moving by dragging" cannot be set.|
|cell format|Some mobiles do not support multiple fonts, so formatting may not work.|

Steps to create and apply mobile pages are:
- Click [Create] → [Mobile Page]. Alternatively, right-click the Pages tab and click Create New Mobile Page.
- Optionally specify whether to allow zooming. Mobile pages are not zoomable by default. If the user wants to enable page zooming, please check "Allow pinch to zoom" from page settings. In addition, when allowing zooming as a subpage of a container control or tab control, be sure to check "Allow zooming by pinch operation" even in the settings of the page where the container control or tab page is placed.
- Change the page name as desired. Rename the page by right-clicking the automatically named page in the Navigation Pane and selecting Rename. At this time, the mobile page is displayed with a different icon than the normal page. The page name of the open page is displayed in the tab under the workspace.

Tip: You can also rename by double-clicking the tab at the bottom of the workspace, just like in Excel.
{:.note}
- Apply mobile pages to regular pages. To automatically display the mobile page when viewing the normal page on mobile, associate the following: Create a normal page and specify the mobile page name you want to display in "Page settings" on the right pane.
