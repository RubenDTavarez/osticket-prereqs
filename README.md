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

- Install/Eneable IIS in Windows with CGI
- PHP Manager for IIS 
- Rewrite Module 
- Microsoft VC++ Redistributable   
- MySQL Data Base

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/7j63LaO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From our VM we are going to install/enable IIS with CGI. This is a websever by Microsoft for hosting websites, apps and services on windows machines. 
To do this we will go to the control panel, look for the icon named "programs" and click righ under it where it says "Uninstall Program" Once this is clicked, 
to the left of the side of our window we will click on "Turn Windows features on or off"  
</p>
<br />


<p>
<img src="https://i.imgur.com/C5Z2jte.png" height="50%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We need to enable feature "Internet Information Services" by clicking on it and selecting it. Once mark, expand on this feature to get to the "Application Development features"
and click on the feature CGI. Once with hit ok, a window will pop up comfirming and installing the features just added. 
</p>
<br />


<p>
<img src="https://i.imgur.com/5Q2mnQ8.png" height="50%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After install/Eneable IIS w/ CGI, there is a list of softwares to be install before with continue with the installation of the osTicket. The first to be install is the PHP Manager for IIS "PHPManagerForIIS_V1.5.0" and the second one is the Rewrite Module (rewrite_amd64_en-US.msi). 
 
<p>  
<img src="https://i.imgur.com/XRgOzX5.png" height="50%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We are going to create a folder in disc C: named "PDP" and in this folder we will extract zip.file 
"php-7.3.8-nts-Win32-VC15-x86.zip" from the list of the requirements files.
</p>   
<br />


<p>
<img src="https://i.imgur.com/mDcvAIO.jpeg" height="50%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
  The next software to Install is the data base "MySQL". This will help us store the users and staff information; also the metadata from the tickets such as subjet, date, status, priorities, etc.  
   - There are some things to do while installing  MySQL; we will select a "typical setup"
   - We are also going to launch configuration Wizard (after install)
   - Standar configuration and we will set our Username and password 

</p>
<br />


<p>
<img src="https://i.imgur.com/20d3R3R.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
   - From our VM open IIS as an administrator and double click on the "PHP Manager" icon. Under the PHP Setup click the option "Registrer New PHP Version" click it and navegate to the PHP folder we created in the local disk "C:". Go to C:\PHP\php-cgi.exe and click "ok" to complete this process we will go back to our main IIS manager window, to the right side we see the "actions tap". To reset our server we will click "stop" and "Star" and this will conclude this step  
</p>
<br />


<p>
<img src="https://i.imgur.com/goMj5M3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
   The next final software to be install is the osTicket but there are some steps to take before installing it. From osTicket installation file folder click on the file name "osTicket-v1.15.8" and extract its content. The file name "upload" will be copy and paste to "c:\inetpub\wwwroot” and rename from "upload" to "osTicket". Once done, reload the IIS and "stop" and "star" the server. 
</p>
<br />


<p>
<img src="https://i.imgur.com/itO2kty.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
   From the IIS manager we will attempt to visit the localhost/osTicket here we will fing of the extensions that are not eneable. From the IIS manager we can click on sites and open the PHP manager under the osTicket folder. Go to PHP and eneable "php_imap.dll", "php_intl.dll" and "php_opcache.dll"   
</p>
<br />


<p>
<img src="https://i.imgur.com/IE0zAaS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/S9Wrmbr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 We need to assign some permissions to the file "ost-config.php" located "C:\inetpub\wwwroot\osTicket\include\ost-config.php" To do this we right click on the file and click on properties, click  on security, highlight "system" and click on the "advanced" On the next window we will click on "Disable inheritance" and remove all inherited permission.
</p>
<br />


<p>
<img src="https://i.imgur.com/quag8BM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  We can go back to the osTicket installer and see that the extension required is enable. Click continue and in the next portal we can continue with the installation on the osTicket. In this new section of the installation we are going to fill out the information required. The Helpdesk name and the email address in charge to receive the emails from the customers.  
</p>
<br />


<p>
<img src="https://i.imgur.com/u1kruzM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  From the "osTicket installation files" folder, install HeidiSQL. This is a tool to allow user to interact with databases using a graphical interface. launch "HeidiSQL" Set a connection to the database by clicking on the "new" here we will use the user and password used to the "MySQL Server" click open and this will set the connection to our database. Now we create a data base for "osTicket"
 <br />






