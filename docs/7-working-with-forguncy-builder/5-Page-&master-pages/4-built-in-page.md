---
layout: default
title: Built-in Page
parent: Page &amp; Master Pages
grand_parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/Page-&-master-pages/built-in-page/
nav_order: 4
---

# {{ page.title }}

When you create a new project, Forguncy automatically prepares pages that are likely to be used frequently in your application as built-in pages and built-in mobile pages in the navigation window.
![built-in-pages](/assets/images/product-images/built-in-pages.png)
{:.dropshadow}

You can either customize these built-in pages as per the requirement or create your own new pages. 

The available built-in pages and built-in mobile pages change depending on the authentication mode specified in the authentication mode settings (refer the below table).
If login fails, check for user authentication modes. It might be different.

#### Table: Built-in Pages and User Authentication Mode

|Built-in page name / Built-in mobile page name|Explanation|Form Authentication|Windows authentication|
|:--|:--|:--|:--|:--|
|401 pages|The page displayes when you access a page for which you do not have permission.|✓|✓|
|Under maintenance now|A page displays temporarily to indicate that it is under maintenance.|✓|✓|
|Password reset|A page for users to reset their passwords.|✓|-|
|Send password reset link|A page that sends password reset emails to users who have forgotten their passwords.|✓|-|
|Change Password|A page where users can change their password.|✓|-|
|If you forget your password|A page that emails you a link for a password reset page, if you forget your password.|✓|-|
|Edit Profile|User profile edit page.|✓|-|
|Email Subscription|Change email notification settings page.|✓|✓|
|Login|login page.|✓|-|

Note: If you change the user authentication mode from Forms authentication to Windows authentication, built-in pages that are not required for Windows authentication will be deleted. 
{:.note}

Even If you have customized a built-in page that has been removed, and you change the user authentication mode back to forms authentication, your previous customizations will not be restored.
{:.note}

##### Page Settings For Built-in Pages

- Selecting and open the built-in page or built-in mobile page that you want to edit from the navigation window
- Click the **Page Settings** tab at the bottom of the right pane to configure:

|Title|Sets the title of the page displayed in the title bar and tabs of the web browser.|
|Master page name|Apply the created master page to the page.|
|Mobile page name|Specifies the mobile page to display when this page is accessed from a mobile device. The built-in mobile page does not display this field.|
|How to display on the master page| Overflow- Show everything beyond the placeholder area.<br/> Scroll- Displays a scrollbar without changing the size of the placeholder. <br/> Cut- Cut the area that extends beyond the placeholder.|
|Number of lines|Sets the number of lines on the page.|
|Number of columns|Sets the number of columns on the page.|
|Page reset|Restore built-in page or built-in mobile page to default state. This setting does not exist on the "Login" page and "Login_Mobile" page.|
|Template selection|You can choose your favorite template from several pattern templates. This setting exists only on the "Login" and "Login_Mobile" pages. <br/> ![built-in-pages](/assets/images/product-images/template-selection.png)|
|Page stretch mode|The page will stretch or shrink depending on the browser at runtime. For more information, see Page stretching.|




