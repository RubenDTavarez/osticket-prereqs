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
<img src="https://i.imgur.com/MkG0B0f.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
   We need to enable feature "Internet Information Services" by clicking on it and selecting it. Once mark, expand on this feature to get to the "Application Development features"
and click on the feature CGI. Once with hit ok, a window will pop up comfirming and installing the features just added. 
</p>
<br />

<p>
<img src="https://i.imgur.com/6IK5UBn.png" height="60%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 After install/Eneable IIS w/ CGI, there is a list of softwares to be install before with continue with the installation of the osTicket. The first to be install is the PHP Manager for IIS "PHPManagerForIIS_V1.5.0" and the
   second one is the Rewrite Module (rewrite_amd64_en-US.msi). 
 <p>  
<img src="https://i.imgur.com/5Q2mnQ8.png" height="60%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />


<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a directory name "PHP" in disk C
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
