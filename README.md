<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>
 
<h2>Installing osTicket on a Windows 11 Virtual Machine</h2>

<h3>What is osTicket</h3>

<t>osTicket is an open-source help desk and ticketing system that lets organizations manage customer support requests by converting emails, phone calls, or web form submissions into organized, trackable tickets.</t>

<h3>About this Project</h3>

In this project we will install and configure osTicket on a virtual machine including it’s prerequisite files and dependencies.

<h3>Environment & Technology Used</h3>

- Microsoft Azure Virtual Machine 
- Microsoft Windows 11
- Remote Desktop

<h3>Prerequisites</h3>

- osTicket-Installation-Files.zip
- PHPManagerForIIS_V1.5.0.msi
- rewrite_amd64_en-US.msi
- php-7.3.8-nts-Win32-VC15-x86.zip
- VC_redist.x86.exe
- mysql-5.5.62-win32.msi
- osTicket-v1.15.8.zip
- HeidiSQL

<h3>Getting Started</h3>

1. Create an Azure Virtual Machine Windows 11, 4 vCPUs (Refer to Azure how to repository link)
     - Name: osticket-vm
     - Username: labuser
     - Password: osTicketPassword1!
       
<mark>NOTE: It is NOT good practice to be putting passwords like this in plain/readable text in any documentation, ever. Best practice is to use a password manager to store passwords, such as KeePass, LastPass, or NordPass. Passwords will continue to be listed in these documents for ease of use, but please just keep security and password managers in mind, especially when it comes to working in the real world.</mark>

