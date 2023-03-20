---
layout: default
title: Create a Master Page
parent: Page &amp; Master Pages
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Page-&-master-pages/create-a-master-page/
nav_order: 3
---

# {{ page.title }}

Use master pages to give your application a uniform look and to organize similarly formatted pages. 

When you apply a master page to a page, that page appears as a child page in a placeholder area within the master page.

A page with a master page applied will have an icon to the right of the page name in the navigation window .

![master-page](/assets/images/product-images/master_page.png)
{:.dropshadow}

You can create master pages for mobile devices. Mobile master pages can only be applied to mobile pages. The creation method and operation are the same as for a normal master page. An icon to the right of the page name in the navigation window will apear.

Note: If the size of the child page is larger than the size of the placeholder on the master page, the child page will be displayed as as per the settings. See [Applying Master Pages](#applying-master-pages) for more information.
{:.note}

Steps to create a new master page:

- Go to **Create** and select **Master Page**.
![create-master-page](/assets/images/product-images/create_master_page.png)
{:.dropshadow}

- Select a template for the master page in the **Select Page Template** dialog. The first template is a top banner and vertical menu, the second template is a top banner and horizontal menu, and the third template is a blank template. 
    
Note: Templates 1 and 2 get affected by theme changes. 
{:.note}

- After selecting a template, click the **OK** button to create a new master page.
- Edit the master page as required.

Note: You can also duplicate an existing master page to create a new master page.
{:.note}

##### Resizing
Resize to change the size of the placeholder:

![create-master-page-resize](/assets/images/product-images/create_master_page_resize.png)
{:.dropshadow}

- Click on the placeholder and select **Design** -> **Start Resize**.
- The **Start Resize** gets converted to **End Resize**. 
- Drag the corners to resize and click on **End Resize** to finish. 
- Apply the master page to child pages. The child pages will show dotted lines in the areas that can be displayed in the placeholder.

If the child page does not fit in the placeholder, you can set **Page Overflow Mode** as *Overflow, Scroll, or Cut* in the page setting of the child page. 

|Overflow|The placeholder expands to fit the size of the child page to show all content.|
|Scroll|A scroll bar appears. It is effective only in the horizontal direction.|
|Cut|The child page is displayed to the size of the placeholder. The protruding part is cut off. It is effective only in the horizontal direction.|

##### Page Setup for Master Pages
- Open the master page you want to edit. 
- Configure settings by clicking on the **Page** tab at the bottom of the right pane.

![create-master-page-settings](/assets/images/product-images/create_master_page_settings.png)
{:.dropshadow}

|**Name**|Sets the name of the master page.|
|**Row count**|Sets the number of rows on the page.|
|**Columns**|Sets the number of columns on the page.|
|**Page stretch mode**|The page will stretch or shrink depending on the browser at runtime.|

## Create a New Mobile Master Page
Steps to create a new mobile master page:

![create-mobile-master-page](/assets/images/product-images/create_mobile_master_page.png)
{:.dropshadow}

- Go to **Create** and click on **Mobile Master Page**.
- Select a template for the master page in the **Select Page Template** dialog. The first template is a top banner and bottom menu, the second template is a blank template. 

Note: The first template gets affected by theme changes.
{:.note}

- After selecting a template, click the **OK** button to create a new mobile master page.
- Edit the master page as required.

Note: You can also clone an existing mobile master page to create a new mobile master page. Right-click on the master page in the Navigation Pane and select **Duplicate**.
{:.note}

##### Resize Placeholder
Child mobile pages appear in the placeholder of the master mobile page. To change the size of the placeholder:

![create-mobile-master-page-resize](/assets/images/product-images/create_mobile_master_page_resize.png)
{:.dropshadow}

Click on the placeholder and select **Design** -> **Start Resize**.
- The **Start Resize** gets converted to **End Resize**. 
- Drag the corners to resize and click on **End Resize** to finish. 
- Apply the master page to child pages. The child pages will show dotted lines in the areas that can be displayed in the placeholder.

If the child page does not fit in the placeholder, you can set **Page Overflow Mode** as *Overflow, Scroll, or Cut* in the page setting of the child page. 

##### Page Setup for Mobile Master Pages
- Open the mobile master page you want to edit. 
- Configure settings by clicking on the **Page** tab at the bottom of the right pane.

![create-mobile-master-page-settings](/assets/images/product-images/create_mobile_master_page_settings.png)
{:.dropshadow}

|**Name**|Sets the name of the mobile master page.|
|**Row count**|Sets the number of rows on the page.|
|**Columns**|Sets the number of columns on the page.|
|**Page stretch mode**|The page will stretch or shrink depending on the browser at runtime.|

## About Built-in Master Pages
When you create a new project in Forguncy, one master page is already available.
You can customize and use this master page as required.

Note: Names cannot be changed or deleted.
{:.note}

Follow the steps mentioned in [Page Setup For Master Pages](#page-setup-for-master-pages) to configure settings.

## Applying Master Pages
You can use master pages to give your pages a consistent look, titles, and common menu items.

- Right-click on the page name.
- Select **Set Master Page** to apply the master page.
- Select the name of the master page to apply. 

When a master page is applied, an icon will appear next to the page name in the Navigation Pane. Icons are different for normal and mobile pages.

Note: Mobile master pages can only be applied to mobile pages. The application method is the same as for a normal master page.
{:.note}

##### Applied Master Page Page Settings
Set the applied master page in the "Page Setup" pane.
This section describes settings related to master pages.


