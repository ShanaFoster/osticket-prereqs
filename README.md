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

- Microsoft Azure Virtual Machine ( Windows 10 2022 64 bit)
- Log into Remote Desktop
- Enabled IIS ( Internet Information service) and CGI
- OsTicket Application Files
- Installation of the PHP Manager, Rewrite
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
The image displayed shows the creation of a Windows 10 2022 64-bit virtual machine in Microsoft Azure. The public IP address obtained from Mircosoft Azure will be used to connect via Remote Desktop, allowing me to install the necessary applications for the OsTicket system.

<br />
</p>
<p>

![image](https://github.com/user-attachments/assets/c6728959-b634-4728-bdf9-d0060ec3972c)
<br />
</p>
The above image shows a Remote Desktop protocol (RDP) session using the public IP address obtained from Mircosoft Azure. This connection is used to remotely access the virtual machine, where the OsTicket system will be installed.

<br />
</p>
<p>

![image](https://github.com/user-attachments/assets/64f740d7-8045-4d5a-bb14-4b143767b21b)
<br />
</p>
The image above shows all the applications required to configure the osTicket system. Fisrt, download the osTicket installation file. Then, open folder,drag it to the desktop, and extract all the files.

<br />
</p>
<p>
  
![image](https://github.com/user-attachments/assets/98981df7-cc36-4e74-ab68-acf443e039f6)
<br />
</p>
The display is shows that the web server failed to connect. I used the loopback IP address (127.0.0.1) to test the connection before enabling IIS (Internet Information Service).

<br />
</p>
<p>

![image](https://github.com/user-attachments/assets/3ee522ad-1a36-445c-93dc-e5fd61ab481d)

![image](https://github.com/user-attachments/assets/532c9acb-8a29-41fc-9a75-0dea680d0faf)

![image](https://github.com/user-attachments/assets/0b5cce87-ce3f-4302-8e74-2d6d17664703)


<br />
</p>
The images above demonstrate how to enable IIS (Internet Information Service) and CGI. I enable IIS by navigating to the Control Panel > programs > Turn Windows features on or off, then select Internet Information Services.

To enable CGI, I navigate to IIS > Application Development > Application Development Features, then select CGI. After completing the steps, I returned to the web server to check the conection.

<br />
</p>
<p>


![image](https://github.com/user-attachments/assets/82f36098-e340-4936-adba-c4d456f22ce4)

![image](https://github.com/user-attachments/assets/9ad66897-d3eb-4afb-8dda-bf250cd55272)

![image](https://github.com/user-attachments/assets/424d9f28-e7ef-43b1-b35a-a8519b4bd984)

![image](https://github.com/user-attachments/assets/6097191d-854e-4c1e-b219-c2373f326e42)

![image](https://github.com/user-attachments/assets/6a91c388-27fa-4c86-ab42-5b9922e3acf2)

<br />
</p>
The images display the applications required to configure the osTicketing system:
-PHPManagerForIIS_V1.5.0, 
-Rewrite_amd64_en-US, 
-VC_redist.x86
-MySQL-5.5.62-win32
 The display also shows essential information in the MySQL server, including the username and password (root), which is required to configure the osTicket system in the HeidiSQL.
  
<br />
</p>
<p>

![image](https://github.com/user-attachments/assets/f695da83-2024-457f-947a-60cf670bfd11)


![image](https://github.com/user-attachments/assets/f6221581-68b5-4c26-b859-f6bb2546da11)


![image](https://github.com/user-attachments/assets/ed84566a-de64-4385-a478-4f14360eeec9)


![image](https://github.com/user-attachments/assets/68ac364b-0ada-458c-9cea-3d6fbc549a94)


</p>
<br />

The image above shows the IIS Manager opened as an administrator. It also display the PHP Manager. i navigate to the PHP Manager and select Register PHP Manager. To register it, I browse to the executable file php-cgi.exe located on the C:drive. After registering PHP Manager, I stop and then restart the web server to apply the changes.
    
<br />
</p>
<p>

![image](https://github.com/user-attachments/assets/15f97f48-67b1-43e5-b6fc-0fcfec60b339)

![image](https://github.com/user-attachments/assets/24473d41-57fd-4b03-934a-c741cb8c684d)

</p>
<br />
The images above demonstrates the Osticket being installed and launched. To install the osTicket, I navigate to the osTicket installation file, extract all contents from osTicket-v1.15.8.zip.This created a second osTicket folder. Iinside that folder, I located upload folder.

I then navigated to the C:drive > Inetpub > wwwroot and I copied the upload folder into wwwrooot. After that, I rename the upload folder to osTicket.

Next I opened IIS manager, reload the server by stoping and restarting it. To launch osTicket, I navigated to Sites > Default Site > osTicket, then select Browse 80 HTTP launch osTicket system. If the system doesn't launch, it means something was configured incorrectly.

<br />
</p>
<p>
  
![image](https://github.com/user-attachments/assets/7d98efa0-5d8b-47a8-bf57-4971a0c777f5)
</p>
<br />

![image](https://github.com/user-attachments/assets/3a86aa01-4ae4-46b6-bd8f-92fae2ef3bc1)

</p>
<br />
The images shows the osTicket system correctly launch but there are some application that are disable that should be enable for that osTicket to properly function.  To enable the required disabled items. I naviagte to IIS manager, select to the PHP manager, and enable the disable items:
- php_imap.dll
- php_intl.dll
- php_opcache.dll

<br />
</p>
<p>
  
![image](https://github.com/user-attachments/assets/715691f0-af77-4206-8585-a63ff8c36576)

![image](https://github.com/user-attachments/assets/e1f6d975-29b5-4c2b-a308-242ed4607de5)

![image](https://github.com/user-attachments/assets/c98b9dcc-4f92-4e6e-8b02-48ade721dce6)

![image](https://github.com/user-attachments/assets/846d0fcd-6f12-49b3-b8c9-bb4f34bb2a29)

The image above demonstrates the Browser folder, which is located on the right.  This folder is where osTiccket is loaded from. To load osTicket, I navigate to Sites > Default Site > osTicket, then select Browse 80 HTTP launch osTicket system. If the system doesn't launch, it means something was configured incorrectly.
<br />
</p>
<p>
  
![image](https://github.com/user-attachments/assets/f331b37f-0a69-4280-a31e-d08e31d6d8c9)

![image](https://github.com/user-attachments/assets/bee8c596-001b-4597-8485-b258ea2b6a7e)


<p>

![image](https://github.com/user-attachments/assets/7b50767c-cedb-4982-b76a-927d8d378e2c)

![image](https://github.com/user-attachments/assets/726e0f15-a742-4b5b-88eb-54f980b80287)

![image](https://github.com/user-attachments/assets/5b0124de-b6b1-403a-b571-667e1c1129f0)


  </p>
<br />

![image](https://github.com/user-attachments/assets/c7a57be6-9d1d-41de-924c-3c30a7e19e9f)

  </p>
<br />

</p>
<p>
This image shows the HeidiSQL database and the information from the HeidiSQl being enetered into the osTicket system. I can use this information to fill out the MySQL section so the OsTicket application will launch properly.

  </p>
<br />

![image](https://github.com/user-attachments/assets/804eb383-f9b3-473b-a377-7ee959e77c7d)

![image](https://github.com/user-attachments/assets/f13c0ae5-ba73-4fcf-8d69-52c501682f58)


The image above show the OsTicket system successfully Configured.
</p>
<br />


</p>
<br />




