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
<img src="https://imgur.com/9a1b67a8-1ed5-4162-8e21-1a501e66bf91" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
After install/Eneable IIS w/ CGI, there is a list of softwares to be install before with continue with the installation of the osTicket. The first to be install is the PHP Manager for IIS "PHPManagerForIIS_V1.5.0" and the second one is the Rewrite Module (rewrite_amd64_en-US.msi). 
 
<p>  
<img src="https://i.imgur.com/5Q2mnQ8.png" height="50%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We are going to create a folder in disc C: named "PDP" and in this folder we will extract zip.file 
"php-7.3.8-nts-Win32-VC15-x86.zip" from the list of the requirements files.
</p>   
<br />


<p>
<img src="https://i.imgur.com/XRgOzX5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />


<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  The next software to Install is the data base "MySQL". This will help us store the users and staff information; also the metadata from the tickets such as subjet, date, status, priorities, etc.  
   - There are some things to do while installing  MySQL; we will select a "typical setup"
   - We are also going to launch configuration Wizard (after install)
   - Standar configuration and we will set our Username and password 

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
   -Open  IIS as an administrator
   - Register PHP from within IIS (PHP Manager -> C:\PHP\php-cgi.exe)
   -Reload IIS ( Open IIS -> Stop -> Star the server
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
   Install osTicket.
</p>
<br />
