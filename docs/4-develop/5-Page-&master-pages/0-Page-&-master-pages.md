---
layout: default
title: Page &amp; Master Pages
parent: Develop
permalink: /develop/Page-&-master-pages/
nav_order: 5
has_children: true
has_toc: true
---

# {{ page.title }}

A page is a *look* that you see in your web browser. You configure your application by creating pages to display or to enter data from tables. 
There are four types of Pages:

![pages](/assets/images/product-images/pages.png)
{:.dropshadow}

|Page|Description|
|:--|:--|
|**Normal Page**|It is a normal page displayed in the web browser of Windows or iPad. <br/> Application operation gets affected when normal pages are displayed on mobile devices (iPhone and Android). So, if you want to display an application on both desktop and mobile, you need to design a mobile page in addition to the normal page. <br/> Normal pages can be stored in folders by creating folders from the **Pages** tab in the Navigation Pane.|
|**Mobile Page**|This is a page for browsers for mobile devices such as iPhone and Android. For Android, the mobile page is displayed regardless of whether it is a smartphone or a tablet. <br/> Mobile pages can be stored in folders by creating folders from the Pages tab in the Navigation Pane.|
|**Master Page**|Used to design a common layout of a page that can be used by multiple pages. The master page is shared by normal pages, and a mobile master page is shared by mobile pages. <br/> Let’s say there is a common header on all pages. By designing this header part on the master page, you don’t have to design the header on every page. <br/> A master page is usually divided into two parts: the cell area and the placeholder area (which displays the child pages). <br/> You can design a common layout in a normal cell area and use placeholder areas to display normal and mobile pages as child pages inside it.|
|**Built-in Page**|When you create a new project, the pages that are likely to be used frequently in your application are automatically included in the project. <br/> Built-in pages include built-in pages and built-in mobile pages, and certain operations automatically display the page. <br/> Let's say your application gets a 401 error, it will automatically jump to the 401 page, and if you need to log in, it will automatically jump to the login page. <br/> You can change the appearance of the built-in page, such as the style, but you cannot remove the interface parts such as the text box for entering passwords and the login button on the login page.|


