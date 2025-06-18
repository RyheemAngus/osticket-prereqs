
Workin  # osticket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- PHP Mangaer for IIS
- MySQL 
- HeidiSQL
- osTicket v1.18

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Enable IIS in Windows with CGI and Common HTTP Features
- Install PHP Manager for IIS (pHP 8.0 recommended)
- Install MySQL Server and create a database for osTicket
- Install C++ Redistributable
- Install osTicket files and configure permissions

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/tmP4oED.png" height="80%" width="80%" alt="IIS Installation"/>
</p>
<p>
<ol> 
<li>Launch Azure Portal and create a Windows 10 Virtual machine</li>
<li>Connect to the VM via Remote Desktop Connetion</li>
<li>Enable IIS in Windows Features (Add roles and Features)</li>
<li>Install Web Platform Installer to add required componets</li>
</ol>
</p>
<br />

<p>
<img src="https://i.imgur.com/5C3JtXJ.png" height="80%" width="80%" alt="PHP Installation"/>
</p>
<p>
<ol start="5">
<li>Download and install PHP Manager for IIS</li>
<li>Download PHP 8.0 and unzip to C:\PHP</li>
<li>Configure IIS to use PHP by registering the PHP verison </li>
<li>Install MySQL Server and create a database named 'osticket'</li>
</p>
<br />

<p>
<img src="https://i.imgur.com/8QnYdQl.png" height="80%" width="80%" alt="osTicket Installation"/>
</p>
<p>
<ol start="9">
<li>Download osTicket from the offical website</li>
<li>Extract and copy the "upload" folder to c:\inetpub\wwwroot, renaming it to "osticket"</li>
<li>Complete the osTicket web installer by configuring database settings</li>
<li>Clean up by deleting the setup folder and setting config permissions'</li>
  </ol>
</p>
<br />
