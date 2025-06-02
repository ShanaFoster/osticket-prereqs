<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>
</p>
<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>List of Prerequisites</h2>

- Remote Desktop
- Enabled IIS ( Internet Information service)
- Enabled CGI
- Installation of the PHP Manager
- Installation of MySQL
- Display of The IIS manager where the Browser 80 http to launch the Osticket application
- Enable appliacte in IIS, navigate to the IIS and selected the 
  PHP manager to enable what was needed to properly installed the OsTicket
- Image of HediSQl database displaying information to correctly launch the OsTicket application 
- OsTicket successful install showing both Agent and User urls

<h2>Installation Steps</h2>

<br />

<img src="https://i.imgur.com/fMhOown.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

The image displays a Remote Desktop connection (RDP) session using the public IP address obtained from Mircosoft Azure, This connection is used to remotely access the virtual machine, which is used to installed OsTicket system.
</p>

<br />
</p>

<p>

<p>
<img src="https://i.imgur.com/8OpsKO6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 


<br />
</p>
<p>
The image above demonstartes how to enable IIS (Internet Information Service). I navigated to the Control Panel, selected Programs clicked turn Windows features on or off; and then enable IIS.
</p>
<br />

<img src="https://i.imgur.com/KiKYDF0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 


<img src="https://i.imgur.com/PgZPu1v.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

</p>

The images above shows CGI being enabled


</p>
<br />
<img src="https://i.imgur.com/bmIsmZC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

The above image shows the PHP Manager being installed.

<br />
</p>


<img src="https://i.imgur.com/GXuENdH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
The image shows the installation of MYSQL. MySQL is essential for logging into the osTicket system. MySQL serves as the database backend. It is required to log in and manage the osTicket database effectively.
  
  <p>

<br />

<img src="https://i.imgur.com/TodoNLz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

The image display the IIS manager, where the 'Browser' folder is located on the right. Inside Browser folder, Browser 80 HTTP is located. Once you click browser 80 HTTP; the osTicket system should launch. If the system doesn't launch, it means something was incorrectly done.

</p>


<br />
</p>

<img src="https://i.imgur.com/Ycfo1V2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This image shows the osTicket installation, but the installed system  has some disabled items. To resolve this, go back to the IIS manager, navigate to the PHP manager, and enable the disable items so that the OsTicket system function properly.
</p>
<br />

<p>
<img src="https://i.imgur.com/D3FDjyG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  </p>
<br />
  <img src="https://i.imgur.com/gnB8aBL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This image shows the HeidiSQL database and the information from the HeidiSQl being enetered into the osTicket system. I can use this information to fill out the MySQL section so the OsTicket application will launch properly.

  </p>
<br />


<img src="https://i.imgur.com/G3lg9HO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

The image above show the Osticket application installed successfully.
</p>
<br />


</p>
<br />




