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
If your system meets the requirements mentioned above, you can proceed with the installation by downloading the latest installer from the [product website](https://www.forguncy.net/){:target="_blank"}. 

### Forguncy Server for Windows

Follow the instructions on the screen as shown below-

![server-install](/assets/images/product-images/server-install.gif)
{: .dropshadow}

Once the product is installed successfully, you can look for **Forguncy Admin Portal** in the installed application list and run it.

The step-by-step procedure of installing Forguncy Server is-

- Open the .exe file and agree to the **User license Agreement**. 
- Give the installation path and click the **Install** button.

![forguncy-server-installation](/assets/images/product-images/forguncy-server-installation.png)
{: .dropshadow}

- It will take some time to initiate and finish the installation. 

![forguncy-server-installation-progress](/assets/images/product-images/forguncy-server-installation-progress.png)
{: .dropshadow}

- Once the installation is finished you can check the *Start up Forguncy Server Admin Portal* to launch the **Server Manager** after closing the popup. 

![forguncy-server-install-finished](/assets/images/product-images/forguncy-server-install-finished.png)
{: .dropshadow}

- Enter credentials to log into the Forguncy server manager. 

![forguncy-server-manager](/assets/images/product-images/forguncy-server-manager.png)
{: .dropshadow}

### Forguncy Server for Linux

The step-by-step procedure of installing Forguncy Server is-

- Check the system requirements and make sure that the environment of the computer you are trying to install meets the system requirements.
- Download the Linux version of Forguncy Server. Access the URL described in the body of the delivery email and download the TAR file, which is the installer archive. If the downloaded file is not on the OS to be installed, transfer the file to the tmp directory of the target environment using the SCP command or FTP.
- Remotely connect to your Linux environment. If you don't have an SSH client installed, you'll need to enable SSH in PowerShell.
- Go to the directory containing the downloaded TAR file.
- Extract the TAR file- *sudo tar -xvf forguncy_linux_x_x_x_x.tar*

![forguncy-server-linux](/assets/images/product-images/forguncy-server-linux.png)
{: .dropshadow}

Note- Here *x* refers to a different version number depending on the version of Forguncy. It can also be the filename *forguncy_linux.tar* without a version number.
{:.note}

- Install Forguncy Server. Execute the extracted SH file with the following command to install Forguncy Server. <br/> *sudo bash installForguncy_en.sh* <br/> Installs various .NET 6 runtimes required at runtime if the target installation has an internet connection enabled. The installation process will take several minutes. <br/>When the installation is complete, the following will be displayed.

![forguncy-server-linux-installed](/assets/images/product-images/forguncy-server-linux-installed.png)
{: .dropshadow}

- A successful installation will install Forguncy Server functionality and the Forguncy Server Management Portal. You can now publish your application to Forguncy Server. You can access the server management portal by accessing the URL in the red frame with a web browser.

![forguncy-server-linux-server-managemen](/assets/images/product-images/forguncy-server-linux-server-management.png)
{: .dropshadow}


## Uninstallation
Open the **Add or remove programs** and select the **Forguncy Admin Portal**. Follow the instruction on the screen, and the software is removed, as shown in the screenshot below. 


![server-uninstall](/assets/images/product-images/server-uninstall.gif)
{: .dropshadow}