<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>
 
<h2>Installing osTicket on a Windows 10 Virtual Machine</h2>

<h2>What is osTicket</h2>

<t>osTicket is an open-source help desk and ticketing system that lets organizations manage customer support requests by converting emails, phone calls, or web form submissions into organized, trackable tickets.</t>
<h2>About this Project</h2>
In this project we will install and deploy osTicket on a Windows 10 virtual machine including it’s prerequisite files and dependencies within Azure.

<h2>Environment & Technology Used</h2>

- Microsoft Azure Virtual Machine 
- Microsoft Windows 10
- Remote Desktop
- PHP
- MySQL

<h2>Prerequisites</h2>

- osTicket-Installation-Files.zip
- PHPManagerForIIS_V1.5.0.msi
- rewrite_amd64_en-US.msi
- php-7.3.8-nts-Win32-VC15-x86.zip
- VC_redist.x86.exe
- mysql-5.5.62-win32.msi
- HeidiSQL

<h2>Getting Started</h2>

<h3>1. Create and log in to a Windows 11 Virtual Machine in Azure with the following Settings and Credentials:</h3>

- VM Name: vm-osTicket
- Operating System: Windows 10 22H2-X64
- Size: 4vCPUs, 32GB Ram (for better performance)
- Username: labuser
- Password: osTicketPassword1!

>[!NOTE]
>_Please refer to  [MS Azure Virtual Machines](https://github.com/pmaglana/azure-active-directory) for detailed instruction on how to create VMs._
      
>[!CAUTION]
>_It is NOT good practice to be putting passwords like this in plain/readable text in any documentation. Best practice is to use a password manager to store passwords, such as KeePass, LastPass, or NordPass. Passwords will continue to be listed in these documents for ease of use, and for training purposes only._</mark>

<h3>2. Log into the Virtual machine with Remote Desktop (ADD LINK)</h3>

Within the vm-osTicket VM, download the [osTicket-Installation-Files.zip](https://drive.google.com/file/d/1YsiGAyLoOjtVyXyeYBJzAu5XdtiGBu0I/view?usp=sharing) and unzip it onto your desktop. The folder should be called “osTicket-Installation-Files”. We will use the files in this folder to install osTicket and some of the dependencies. SS below for the complete file list.

<details><summary>See screenshots</summary>
<img src="images/procedure1.png" width="40%" >
</details> 

<h3>3.  Enable IIS in Windows with CGI</h3>
