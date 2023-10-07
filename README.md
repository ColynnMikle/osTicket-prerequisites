<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
Outlined is a summary of the installation of osTicket, as well as the necessary files and processes for it's operation.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Enable Internet Information Services/CGI/Common Http
- Enable IIS Management Console 
- PHP Manager for IIS
- Rewrite Module
- Ensure that C: PHP directory file is active
- PHP 7.3.8
- VC redist.x86.exe
- MySQL 5.5.62
- osTicket v1.15.8
- HeidiSQL
<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From within Control Panel, Internet Information Services must be enabled. World Wide Web Services dropdown menus should be used to enable CGI and Common http features. IIS Management Console must be enabled to allow access to IIS window later.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create C: directory file entitled "PHP". Download the files listed above until MySQL is reached. Run installation wizards to complete installation. Note: When PHP 7.3.8 is installed, files should be extracted to C:PHP directory. Once files up to MySQL have been installed, open the IIS window enabled earlier as an admin and register PHP. Install osTicket v1.15.8. Once finished, Restart IIS using the appropriate link. Then proceed to the "Sites" tab and find osTicket tab. Access PHP manager from this page and enable php_imap, php_intl, and php_opcache. IIS page in browser (accessed from the "Browse*:80" tab from main IIS window) should default to osTicket page.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From within inetpub folder in C: directory, rename "ost-sampleconfig.php" to "ost-config.php". Disable Inheritance properties, and enable Permissions to allow All, Everyone, or those with desired access as needed. Install Heidi SQL and create database called "osTicket". Complete osTicket setup inside browser using credentials created. 
</p>
<br />
