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



![image](https://github.com/user-attachments/assets/aca4c194-3abf-46a9-9365-0c6db79e8103)

<br />
</p>
The image display is of the Windows 10 2022 64bit virtual machine being created in Microsoft Azure. The public IP address obtained from Mircosoft Azure, will then be used to connect to the remote desktop so we can install the neccessary application for the  installed OsTicket system.
</p>
<p>

![image](https://github.com/user-attachments/assets/c6728959-b634-4728-bdf9-d0060ec3972c)

<br />
</p>
<p>
The image displays a Remote Desktop connection (RDP) session using the public IP address obtained from Mircosoft Azure, This connection is used to remotely access the virtual machine, which is used to installed OsTicket system.
</p>

<br />
</p>

<p>

<p>

![image](https://github.com/user-attachments/assets/98981df7-cc36-4e74-ab68-acf443e039f6)

<br />
</p>
<p>
The image displays Loop back IP addressession  remotely access the virtual machine, which is used to installed OsTicket system.
</p>
<br />
<p>

![image](https://github.com/user-attachments/assets/3ee522ad-1a36-445c-93dc-e5fd61ab481d)

  
The image above demonstartes how to enable IIS (Internet Information Service). I navigated to the Control Panel, selected Programs clicked turn Windows features on or off; and then enable IIS.
</p>
<br />


![image](https://github.com/user-attachments/assets/532c9acb-8a29-41fc-9a75-0dea680d0faf)

</p>
<br />

![image](https://github.com/user-attachments/assets/0b5cce87-ce3f-4302-8e74-2d6d17664703)


The images above shows CGI being enabled and 

</p>
<br />

![image](https://github.com/user-attachments/assets/64f740d7-8045-4d5a-bb14-4b143767b21b)

</p>
<p>
The above image shows all the applications needs to configure the OsTicket system.
 </p>
<br />


![image](https://github.com/user-attachments/assets/82f36098-e340-4936-adba-c4d456f22ce4)

![image](https://github.com/user-attachments/assets/9ad66897-d3eb-4afb-8dda-bf250cd55272)

![image](https://github.com/user-attachments/assets/424d9f28-e7ef-43b1-b35a-a8519b4bd984)

![image](https://github.com/user-attachments/assets/6097191d-854e-4c1e-b219-c2373f326e42)

<br />
</p>
The image shows the installation of MYSQL. MySQL is essential for logging into the osTicket system. MySQL serves as the database backend. It is required to log in and manage the osTicket database effectively.
  
  <p>
<br />

<img src="https://i.imgur.com/TodoNLz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
</p>
The image display the IIS manager, where the 'Browser' folder is located on the right. Inside Browser folder, Browser 80 HTTP is located. Once you click browser 80 HTTP; the osTicket system should launch. If the system doesn't launch, it means something was incorrectly done.

<br />
</p>

![image](https://github.com/user-attachments/assets/f695da83-2024-457f-947a-60cf670bfd11)



The image display the IIS manager being open and run as administrator 

</p>

![image](https://github.com/user-attachments/assets/f6221581-68b5-4c26-b859-f6bb2546da11)


![image](https://github.com/user-attachments/assets/ed84566a-de64-4385-a478-4f14360eeec9)


![image](https://github.com/user-attachments/assets/68ac364b-0ada-458c-9cea-3d6fbc549a94)



</p>
<br />

his image shows the osTicket installation, but the installed system  has some disabled items. To resolve this, go back to the IIS manager, navigate to the PHP manager, and enable the disable items so that the OsTicket system function properly.
</p>

</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/24473d41-57fd-4b03-934a-c741cb8c684d)

</p>
<br />
The image display the IIS manager, where the 'Browser' folder is located on the right. Inside Browser folder, Browser 80 HTTP is located. Once you click browser 80 HTTP; the osTicket system should launch. If the system doesn't launch, it means something was incorrectly done.
<p>
  
</p>
<br />
  
![image](https://github.com/user-attachments/assets/7d98efa0-5d8b-47a8-bf57-4971a0c777f5)
</p>
<br />

![image](https://github.com/user-attachments/assets/3a86aa01-4ae4-46b6-bd8f-92fae2ef3bc1)

</p>
<p>
This image shows the osTicket installation, but the installed system  has some disabled items. To resolve this, go back to the IIS manager, navigate to the PHP manager, and enable the disable items so that the OsTicket system function properly.
</p>
<br />


![image](https://github.com/user-attachments/assets/f331b37f-0a69-4280-a31e-d08e31d6d8c9)

![image](https://github.com/user-attachments/assets/bee8c596-001b-4597-8485-b258ea2b6a7e)


<p>

![image](https://github.com/user-attachments/assets/7b50767c-cedb-4982-b76a-927d8d378e2c)

![image](https://github.com/user-attachments/assets/b3fcdae6-f61d-4aee-bd4a-03c5d202e2f8)


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




