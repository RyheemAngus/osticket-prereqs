<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- PHP Manager for IIS
- Rewrite Module
- PHP 7.3.8
- VC_redist.x86
- MySQL 5.5.62
- HeidiSQL
- osTicket v1.15.8

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2></h2>Azure VM Setup</p>h2>

Create a Windows 10 VM with:
- Name: osticket-vm
- Username: labuser
- Password: osTicketPassword1!

Then I proceeded to log into the virtual machine wwith remote desktop.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Install Dependencies</h2>

Firstly I had to ensure I enabled and installed the correct programs to allow osTicket to work.

- I had to install and enable IIS with CGI 
- Then I installed PHP Manager for IIS 
- I installed Rewrite Module 
- I installed VC_redist.x86
- I also had to exract my PHP files which then enabled me to access the file below. 

I also installed and set up MySQL 5.5.62 with:
- I selected typical set up
- Username: root
- Password: ROOT
Later on I encountered some trouble with the password, but the solution was making the whole password capital letters rather than just the R. 
</p>
<br />

<p>
<h2>osTicket Deployment</h2>

Unzip osTicket-v1.15.8.zip → Copy upload folder to C:\inetpub\wwwroot → Rename to osTicket.
Screenshot:
File Explorer showing the renamed osTicket folder in wwwroot.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Configure IIS</h2>

Register PHP in IIS (PHP Manager → C:\PHP\php-cgi.exe).
Enable extensions:
php_imap.dll
php_intl.dll
php_opcache.dll
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Finalize osTicket</h2>

Rename ost-sampleconfig.php to ost-config.php.
Set permissions: Everyone → Full Control.
Create database in HeidiSQL:
sql
CREATE DATABASE osTicket
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Complete setup</h2>

Access osTicket at http://localhost/osTicket/scp/login.php
</p>
<br />
