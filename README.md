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
- OsTicket Installation Files
- Registered PHP Manager
- Launch osTicket and enbled the disabled application in the PHP Manager
- Add permission for Everyone to again access to osTicket
- Setup OsTicket with Help Desktop and Admin information
- Installed HediSQl database and in fill in the required information
- OsTicket successfully installed showing both Agent and User urls

<h2>Installation Steps</h2>

<br />



![image](https://github.com/user-attachments/assets/aca4c194-3abf-46a9-9365-0c6db79e8103)
<br />
</p>
Microsoft Azure is Microsoft’s cloud platform that lets you store and process data without physical hardware. You only pay for what you use. Companies create a resource group to organize resources, which must exist before creating a virtual machine. The image shows a Windows 10 2022 64-bit virtual machine in Azure. The public IP address was used to connect via Remote Desktop. After completing the task, I deleted the resource group, which removed all resources and helped save costs.


<br />
</p>
<p>

![image](https://github.com/user-attachments/assets/c6728959-b634-4728-bdf9-d0060ec3972c)
<br />
</p>

Remote Desktop Protocol (RDP) primarily uses Transmission Control Protocol (TCP) on port 3389. It enables a remote connection between a client and a host system, allowing users to control and access a device as if they were physically present. The image demonstrates an active Remote Desktop session using a public IP address provided by Microsoft Azure. This connection is used to remotely access the virtual machine.

<br />
</p>
<p>

![image](https://github.com/user-attachments/assets/64f740d7-8045-4d5a-bb14-4b143767b21b)
<br />
</p>

osTicket is a cost-effective system for managing customer communication and support. It also keeps both customers and staff accountable. To use osTicket, some applications need to be installed. The image above shows the steps: first, download the osTicket installation file. Then, open the folder, drag it to the desktop, and extract all the files needed to install osTicket.


<br />
</p>
<p>
  
![image](https://github.com/user-attachments/assets/98981df7-cc36-4e74-ab68-acf443e039f6)
<br />
</p>

The loopback address is used to check the function of your computer’s network. The image above shows the loopback IP address (127.0.0.1) being used for testing before Internet Information Services (IIS) is enabled.

<br />
</p>
<p>

![image](https://github.com/user-attachments/assets/3ee522ad-1a36-445c-93dc-e5fd61ab481d)

![image](https://github.com/user-attachments/assets/532c9acb-8a29-41fc-9a75-0dea680d0faf)

![image](https://github.com/user-attachments/assets/0b5cce87-ce3f-4302-8e74-2d6d17664703)


<br />
</p>

Internet Information Services (IIS) and Computer-Generated Imagery (CGI) can be enabled by navigating to Control Panel > Programs > Turn Windows features on or off, and then selecting Internet Information Services.

To enable CGI, I navigated to IIS > Application Development > Application Development Features, and then selected CGI. After completing these steps, I returned to the web server to check the connection, as shown above, to confirm that IIS and CGI were enabled.

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


The osTicketing system is a web-based help desk that needs several applications to work correctly. These include the list of application below wihich shows the images above. 

-PHPManagerForIIS_V1.5.0 ,
-Rewrite_amd64_en-US ,
-VC_redist.x86 ,
-MySQL-5.5.62-win32

The system also shows important MySQL server details, such as the root username and password, which is required to setup the osTicket database using HeidiSQL.
  
<br />
</p>
<p>

![image](https://github.com/user-attachments/assets/f695da83-2024-457f-947a-60cf670bfd11)


![image](https://github.com/user-attachments/assets/f6221581-68b5-4c26-b859-f6bb2546da11)


![image](https://github.com/user-attachments/assets/ed84566a-de64-4385-a478-4f14360eeec9)


![image](https://github.com/user-attachments/assets/68ac364b-0ada-458c-9cea-3d6fbc549a94)


</p>
<br />



PHP Manager plays an important role in the osTicketing system. After installing it, registration is required. I open the Control Panel, select IIS, and run it as an administrator. Once IIS opens, I select Register PHP Manager and browse to the executable file php-cgi.exe located on the C: drive. After registering PHP Manager, I stop and restart the web server to apply the changes.
<br />
</p>
<p>

![image](https://github.com/user-attachments/assets/30f77e51-36d4-490a-86c9-a04bf2fab63d)

![image](https://github.com/user-attachments/assets/15f97f48-67b1-43e5-b6fc-0fcfec60b339)

![image](https://github.com/user-attachments/assets/24473d41-57fd-4b03-934a-c741cb8c684d)

</p>
<br />

The images above demonstrates the osticket being installed and launched. To install the osTicket, I navigate to the osTicket installation file, extract all contents from osTicket-v1.15.8.This created a second osTicket folder. Inside that folder, I located upload folder.

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
After the osTicket is be launch some application were disable that should be enable for the osTicket to properly function.  To enable the required disabled items. I naviagte to IIS manager, select to the PHP manager, and enable the disable items:
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


To grant everyone permission to make changes to the osTicket system I follow these steps:

File explorer > 

*C:\inetpub\wwwroot\osTicket\include*

Located the file ost-sampleconfig.php right click and rename it to ost-config.php.

Right-clicked the file and selected Properties.

Opened the Security tab and clicked Advanced.

Disabled inherited permissions by selecting Disable inheritance.

Added a new permission entry.

In the Principal field, selected Everyone.

Assigned Full Control permissions.

Clicked OK and applied the changes.

Giving access to everyone is not permitted in the real world for security reasons.

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
The HeidiSQL database is needed to complete the setting up of the osTicket system. After installing the HeidiSQL application which is located in the osTicket installation folder. I opened HeidiSQL to create a new connection and entered the Username and Password (both sets as root), which I had configured in MySQL server. 
Then, I created a database call osTicket by navigating to the dophin icon in the HeidiSQL application, selected create new > Database, named it osTicket, and clicked Ok to apply the changes. 

 I then returned to the osTicket setup screen and entered the following information below in the database.
 - MYSQL Database : osTicket
 - MySQL User : root
 - MySQL Password : root
  
Then, I clicked install now to complete the osTicket system setup.

 </p>
<br />

![image](https://github.com/user-attachments/assets/804eb383-f9b3-473b-a377-7ee959e77c7d)

![image](https://github.com/user-attachments/assets/f13c0ae5-ba73-4fcf-8d69-52c501682f58)


The image above shows the osTicket system has been successfully configured.
</p>
<br />


</p>
<br />




