---
layout: default
title: App Publishing
parent: Working with Forguncy Server
permalink: /working-with-forguncy-server/app-publishing/
nav_order: 1
has_children: true
has_toc: true
---

# {{ page.title }}

To make your applications available to end users, you need to publish them using Forguncy server. 

Once the app development is finished in forguncy Builder read below section for the step by step procedure of online app publishing.

<!-- Applications can be published on the server using one of two methods:

- Publishing directly from Forguncy Builder to Forguncy Server over the network.
- Deploying apps offline (applicable for Windows version of Forguncy server only) -->

It is recommended to install Forguncy Server in advance on the computer system where you will publish the application,　and add users if necessary.

Application publishing uses TCP port 22345. When Forguncy Server is installed, the required settings to allow communication of 22345 port number is automatically added to the firewall settings of the OS. If you face any issues while publishing your application, please check if TCP port 22345 is allowed or not. 

The following is an example of the setting method for Windows-

- From the control panel of the destination computer, go to *\System and Security\Windows Firewall* and open Windows Firewall.
- Click **Advanced Settings** on the left and open **Windows Firewall with Advanced Security**.
- Click on **Inbound Rules** to display it.
- Find the inbound rule named *Forguncy22345* from the displayed inbound rules. The port number 22345 is used at the time of issuance, so it cannot be issued if this inbound rule is disabled.

If the above port number is enabled and you are still unable to connect to the server, then there is a possibility that access to this port number may be restricted somewhere else. Check with the person in charge (system administration department) of network administration whether this port number is accessible or not.

