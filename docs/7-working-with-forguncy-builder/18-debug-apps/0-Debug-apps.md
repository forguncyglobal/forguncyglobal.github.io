---
layout: default
title: Debug Apps
parent: Working with Forguncy Builder
permalink: /working-with-forguncy-builder/debug-apps/
nav_order: 18
has_children: true
has_toc: true
---

# {{ page.title }}

Forguncy has a built-in web server. You can check the appearance and operation of the application under development on a web browser.
You can also check the look and feel of the app when viewed on a mobile device.

Note: If you don't want to see the login screen while debugging, you can disable it. Read [Disable login screen](https://docs.forguncy.net/working-with-forguncy-builder/Project/loading-and-running-the-project/#disable-login-screen).
{:.note}

Steps to debug the application on Forguncy web server are:

- Go to **Home** tab and click the **Start** button.

![debug-app-start](/assets/images/product-images/debug-app-start.png)
{:.dropshadow}

- The application being created is displayed in a web browser (in the same state as when it will be published).
- To select the web browser to display, click **Start** drop-down button and select the desired web browser.

![debug-app-web-browser-selection](/assets/images/product-images/debug-app-web-browser-selection.png)
{:.dropshadow}

<!-- If you hold down the *Ctrl* key and click the **Start** button, you can check that the hidden rows/columns are displayed. -->

- If the database data is changed from the application during debugging, a message dialog will appear, and you can select whether to reflect the changed data to the internal database on Forguncy Builder.

![debug-start-data-modified](/assets/images/product-images/debug-start-data-modified.png)
{:.dropshadow}

This dialog is also displayed when you change the data of the external database. But in the case of external databases, the data is reflected in real time regardless of the button clicked in this dialog. In addition, it is possible to set whether or not to display this dialog in the environment setting of the option .

Note: If your application is saved in a project (FGCP) file, you don't need to click the Start Debugging button again when modifying your application. Click the save button to save the project, reload the page in your web browser, and your modifications will be reflected.
{:.note}

Select a cell in your web browser and press *Ctrl+M* to see the cell name. If the cell is unnamed, the ID will be displayed. Release the key and the cell name or ID will disappear. This feature is useful when debugging applications that use JavaScript APIs.

## Check Mobile Device Display

You can also see how your application will look and behave on mobile devices. However, the display state will not be exactly the same on mobile devices as on the web browser of the computer, such as scroll bars will appear on the mobile screen.

Steps to check the appearance of an application on the mobile device are:

- Go to **Home** tab and click the **Start** button.
- Select **Mobile simulator** from the dropdown.
- The mobile device layout of the application will appear in the web browser.

![debug-mobile-device](/assets/images/product-images/debug-mobile-device.png)
{:.dropshadow}

