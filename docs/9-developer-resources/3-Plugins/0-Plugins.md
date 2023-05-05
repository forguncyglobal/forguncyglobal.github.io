---
layout: default
title: Plugins
parent: Developer Resources
permalink: /developer-resources/plugins/
nav_order: 3
has_children: true
has_toc: true
---

# {{ page.title }}

By using plugins, you can extend the functionality of Forguncy by adding more cell types and commands.

Plugins include pre-installed plugins that are included in the Forguncy installer and can be used immediately after installing Forguncy, and plugins that need to be [downloaded](#downlod-plugins) and installed separately. It is also possible to install third party plugins that are not created by Forguncy team.

Note: The plugin is also published with the application. No special action is required while publishing an application in the case of plugins.
{:.note}

## Downlod Plugins

Each plugin download file below are in ZIP format. Once you download and install it successfully, it will appear in the Plugins section of the Builder. 

If the plugin that you have downloaded provides cell types, you'll notice a new cell type listed in the cell type section. Similarly, if the plugin that you have downloaded provides commands, you'll notice additional commands in the list of Forguncy commands.

|Title|Download|
|:-- |:--: |:--:|
|**ActiveReports Viewer Command:**<br>Displays the ActiveReportsJS report on the browser.|[Download](/assets/plugins/ActiveReportsViewerCommand.zip)|
|**Connect to Box Command:**<br>Provides access to the Box cloud storage.|[Download](/assets/plugins/BoxService.zip)|
|**Carousel Cell Type:**<br>A cell type that cycles through images, like a carousel.|[Download](/assets/plugins/CarouselCellType.zip)|
|**Detect OS Info Command:**<br>Fetches the operating system information.|[Download](/assets/plugins/DetectOSInfoCommand.zip)|
|**Element UI Cell Type:**<br>Provides Element UI components as cell types.|[Download](/assets/plugins/ElementUI.zip)|
|**Encrypt & Decrypt Command:**<br>Performs various encryption and decryption.|[Download](/assets/plugins/EncryptDecryptCommand.zip)|
|**File Previewer Cell Type:**<br>Preview the uploaded files in a browser directly.|[Download](/assets/plugins/FilePreviewer.zip)|
|**Menu & Treeview Cell Type:**<br>Provides menus and treview UI components.|[Download](/assets/plugins/Forguncy.CustomMenu.zip)|
|**Pass Listview Data Command:**<br>Passes data from one listview to the another.|[Download](/assets/plugins/PassListviewDataCommand.zip)|
|**Gantt Cell Type:**<br>Provides a Gantt view UI component.|[Download](/assets/plugins/Gantt.zip)|
|**HTML Rich Editor Cell Type:**<br>Edit HTML text in a rich editor.|[Download](/assets/plugins/HtmlRichEdtior.zip)|
|**Image Editor Cell Type:**<br>Image editor.|[Download](/assets/plugins/ImageEditor.zip)|
|**Image Viewer Cell Type:**<br>Image viewer.|[Download](/assets/plugins/ImageViewerCommand.zip)|
|**Import Export CSV Command:**<br>Import or export data from or to CSV file.|[Download](/assets/plugins/ImportExportCSV.zip)|
|**JSON Data Source Command:**<br>Use JSON data on listview or cell.|[Download](/assets/plugins/JsonDataSource.zip)|
|**JSON Serializer Command:**<br>Serialize or deserialize JSON data.|[Download](/assets/plugins/JsonUtilityCommand.zip)|
|**Loading Animation Command:**<br>Provides animation to give feedback to the end user to wait.|[Download](/assets/plugins/LoadingCommand.zip)|
|**Office365 Login Command:**<br>Provides a way to authenticate with Office365 acocunts.|[Download](/assets/plugins/Office365LoginCommand.zip)|
|**Connect to OneDrive Command:**<br>Provides access to the OneDrive cloud storage.|[Download](/assets/plugins/OneDriveService.zip)|
|**Scan WeChat QR Code:**<br>Scans WeChat QR code for login (un-supported in India).|[Download](/assets/plugins/OpenWeChatCommand.zip)|
|**Operate Files Command:**<br>Provides commands to perform various actions on a file.|[Download](/assets/plugins/OperateFilesCommand.zip)|
|**Reload Listview Command:**<br>Performs a series of commands necessary to reload listview properly.|[Download](/assets/plugins/ReloadListViewCommand.zip)|
|**Selection Panel Cell Type:**<br>Displays the items selected in a Listview.|[Download](/assets/plugins/SelectionPanel.zip)|
|**Send DingTalk Message:**<br>Sends DingTalk message.|[Download](/assets/plugins/SendDingTalkMessage.zip)|
|**Send HTTP Request Command:**<br>Perform raw HTTP requests.|[Download](/assets/plugins/SendHTTPRequestCommand.zip)|
|**Send WeChat Message Command:**<br>Sends WeChat messages.|[Download](/assets/plugins/SendWeChatMessage.zip)|
|**Set Cell Location Command:**<br>Changes the current cell to the location you specify.|[Download](/assets/plugins/SetCellLocationCommand.zip)|
|**Set Current Row Command:**<br>Changes the current row to the row you specify.|[Download](/assets/plugins/SetCurrentRowCommand.zip)|
|**Set Focus Command:**<br>Allows you to maintain focus on a cell while command executes.|[Download](/assets/plugins/SetFocusCommand.zip)|
|**Signature Cell Type:**<br>Show signature on a web page.|[Download](/assets/plugins/SignatureCellType.zip)|
|**Wait Command:**<br>Performs a wait (or sleep) operation for a specified duration.|[Download](/assets/plugins/SleepCommand.zip)|
|**Scan QR Command:**<br>Scans a QR code and places the fetched data on a cell.|[Download](/assets/plugins/SmartPhoneCommand.zip)|
|**Tab Cell Type and Command:**<br>Provides tab on a page as well as can perform opening a link on a new tab on a browser.|[Download](/assets/plugins/TabManager.zip)|
|**Message Microsoft Teams Command:**<br>Sends a message to the Microsoft Teams.|[Download](/assets/plugins/TeamsWebHookCommand.zip)|
|**Trace Process Status Command:**<br>Traces and logs the status of a process.|[Download](/assets/plugins/TraceProcessStatusCommand.zip)|
|**User Management Command:**<br>Provides commands for uer management.|[Download](/assets/plugins/UserManagementCommands.zip)|
|**Vant Cell Type:**<br>Provides Vant UI components.|[Download](/assets/plugins/Vant.zip)|
|**Video Player Cell Type:**<br>A video player.|[Download](/assets/plugins/VideoPlayCellType.zip)|
|**Workflow Command:**<br>Provides workflow.|[Download](/assets/plugins)|

Plugins can only be used with the version of Forguncy that the plugin vouches for. If you install it on an uncertified version of Forguncy, an error dialog will appear and the installation will fail.
{:.note}

If you have an older version of the plugin installed, installing a newer version of the plugin will display a warning dialog asking if you want to replace the older version. Select *Yes* to replace.
{:note}

If the corresponding version of the plug-in is not installed while opening a project file containing an older version of a plugin is not installed, opening a project file containing an older version of a plugin will display an *Install Plugin* dialog. 

The plugin information for older versions is displayed in red. 
When the corresponding version of the plugin is not installed, clicking on the *Cancel* button will delete the cell or command containing the plugin. Therefore, you should install the new version of the plugin beforehand.


