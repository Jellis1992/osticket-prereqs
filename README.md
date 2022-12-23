<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Enable IIS 
- Web Platform Installing 
- MySQL
- Configure permissions/ Install osTicket

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/QbBnpFN.png"/>
  
  - Open after installation
  - Add MySQL 5.5
  - Add All simple versions of x86 PHP up until 7.3
  
</p>
<p>

</p>
<br />

<p>
<img src="https://i.imgur.com/VgZSkie.png"/>
  
  - Reload IIS
  - Go to sites -> Default -> osTicket
  - Double-click PHP Manager
  - Click “Enable or disable an extension”
  - Enable: php_imap.dll
  - Enable: php_intl.dll
  - Enable: php_opcache.dll
</p>
<p>

</p>
<br />

<p>
<img src="https://i.imgur.com/tVmTJxs.png"/>
  
  - Download and Install HeidiSQL  
  - Create a new session, root/Password1 
  - Connect to the session 
  - Create a database called “osTicket”
  
</p>
<p>

</p>
<br />

<img src="https://i.imgur.com/StZcrUG.png"/>

  - Rename: 	From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php 	To: C:\inetpub\wwwroot\osTicket\include\ost-config.php 
  - Assign Permissions: ost-config.php 
    Disable inheritance -> Remove All 
    New Permissions -> Everyone -> All


