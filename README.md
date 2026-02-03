<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>
 
<h2>Installing osTicket on a Windows 11 Virtual Machine</h2>

<h2>What is osTicket</h2>

<t>osTicket is an open-source help desk and ticketing system that lets organizations manage customer support requests by converting emails, phone calls, or web form submissions into organized, trackable tickets.</t>
<h2>About this Project</h2>
In this project we will install and deploy osTicket on a Windows 11 virtual machine including it’s prerequisite files and dependencies within Azure.

<h2>Environment & Technology Used</h2>

- Microsoft Azure Virtual Machine 
- Microsoft Windows 11
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

<h3>1. Create and log in to a Windows 11 Virtual Machine in Azure with the following Name and Credentials:</h3>
     - Name: osticket-vm
     - Username: labuser
     - Password: osTicketPassword1!
       
>[!NOTE]
>It is NOT good practice to be putting passwords like this in plain/readable text in any documentation, ever. Best practice is to use a password manager to store passwords, such as KeePass, LastPass, or NordPass. Passwords will continue to be listed in these documents for ease of use, but please just keep security and password managers in mind, especially when it comes to working in the real world.</mark>

<h3>2. Log into the Virtual machine with Remote Desktop</h3>

Remote Desktop Connect(RDP) to the newly created VM, download the osTicket-Installation-Files.zip from the repo and unzip the whole folder unto your VM desktop. Search the start menu for "Turn Windows features on or off". In the pop-up find Internet Information Services and mark the checkbox. Expand World Wide Web > Expand Application Development Features, find CGI and mark the checkbox, and select OK and wait for features to be installed.

<details><summary>See screenshots</summary>
<img src="images/Step 2a.PNG" width="40%" >
</details> 
