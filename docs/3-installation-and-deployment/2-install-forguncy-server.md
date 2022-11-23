---
layout: default
title: Install Forguncy Server
parent: Installation and Deployment
permalink: /installation-and-deployment/install-forguncy-server/
nav_order: 2
---

# {{ page.title }}


## Before You Install
The Forguncy Server runs on Microsoft Windows operating systems and Linux operating systems. Following are the system requirements you need to keep in mind before installing.

### Operating System (64-bit)
- Windows 7, 8.1 (Update), 10, or 11
- Windows Server 2008 (R2 SP1), 2012, 2012 (R2 Update), 2016, 2019 or 2022
- Ubuntu 16.04, or 18.04
- CentOS 7 (1804)
- RedHat 7.6

The Windows Server Core and Nano Server are not supported.
{: .note}

### Web Browsers
- Internet Explorer 11
- Microsoft Edge (latest)
- Google Chrome (latest)

### Hardware
- CPU: Core™ i3 2GHz or above
- Memory: 4GB or more
- Hard Drive: at least 300MB of free space

A 2GB or more free space is required on your hard drive if .NET Framework is not installed.
{: .note}

### .NET Frameworks
- .NET Framework v4.7.2 or above (the installer for Builder installs automatically if not found installed)
- .NET Core v3.1.4 or above

The system must have .NET Framework 3.5 SP1 or above already installed. If not, you must install it from the [Microsoft webiste](https://dotnet.microsoft.com/en-us/download/dotnet-framework/net35-sp1){:target="_blank"} first.
{: .note}

## Installation
If your system meets the requirements mentioned above, you can proceed with the installation by downloading the latest installer from the [product website](https://www.forguncy.net/){:target="_blank"}. Follow the instructions on the screen as shown below.

![server-install](/assets/images/product-images/server-install.gif)
{: .dropshadow}

Once the product is installed successfully, you can look for **Forguncy Admin Portal** in the installed application list and run it.

## Uninstallation
Open the **Add or remove programs** and select the **Forguncy Admin Portal**. Follow the instruction on the screen, and the software is removed, as shown in the screenshot below. 


![server-uninstall](/assets/images/product-images/server-uninstall.gif)
{: .dropshadow}