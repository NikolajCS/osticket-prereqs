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

- Item 1 Install and enable IIS + CGI in windows features
- Item 2 Install PHP Manager + Rewrite Module
- Item 3 Install Microsoft Visual C++ Redistributable x86, VC_redist.x86.exe.
- Item 4 Install MySQL, (mysql-5.5.62-win32.msi) Typical Setup -> Standard Configuration
- Download PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip)
- Download osTicket https://osticket.com/download/


<h2>Installation Steps</h2>

<p>
<img src="![image](https://github.com/user-attachments/assets/d95f32e3-821a-4352-a31b-61765525f14f)
"/>
</p>
<p>

Open up Windows Features -> Enable IIS (Internet Information Services) ->  Expand it -> Expand World Wide Web -> Expand Application Devolepment Features and enable CGI. 


![image](https://github.com/user-attachments/assets/c9288e02-0d7b-4c81-a3b2-438a42a01160)



Install PHP Manager, (PHPManagerForIIS_V1.5.0.msi)


![image](https://github.com/user-attachments/assets/b3426c48-a041-4c78-9611-6cb75de35fcd)



Install Rewrite Module, (rewrite_amd64_en-US.msi)


![image](https://github.com/user-attachments/assets/bb998225-8ce2-4ec8-8228-9beb688d8dee)



Create the directory C:\PHP -> Open File Explorer -> Open C Drive and create a new folder within the C drive and name it PHP



![image](https://github.com/user-attachments/assets/45c705f2-9d0d-4a4a-8746-58a361499577)

Unzip PHP 7.3.8 -> Extract all -> Browse -> Select The folder PHP 

![image](https://github.com/user-attachments/assets/75fbb65d-e3f6-45d5-889d-0986ba907bb6)



 Install Microsoft Visual C++ Redistributable x86, VC_redist.x86.exe.
 

![image](https://github.com/user-attachments/assets/bc010c84-3283-4bad-974a-636ad1b0c230)


Install MySQL, (mysql-5.5.62-win32.msi) Typical Setup -> Standard Configuration


 ![image](https://github.com/user-attachments/assets/c176992f-19d7-4f2e-a693-436f28c7fcf6)


Now open IIS as an Admin -> click on PHP Manager within IIS -> and then click on register new PHP Version -> locate the php folder we created on the C drive and select the Application within in PHP folder "php-cgi"


![image](https://github.com/user-attachments/assets/28c757bd-dbe0-47b5-8237-571e6ac59b7a)

Extract osTicket -> Then move the upload folder into “c:\inetpub\wwwroot -> Then rename the "upload" folder to "osTicket"


![image](https://github.com/user-attachments/assets/5fc2c1c3-186b-4f38-b286-1a951ca79795)

You will need to reload IIS. Stop the server and start it.
Inside IIS Manager expand osTicket -> Sites -> Default Web site -> click on osTicket -> Browse *:80 (http)

![image](https://github.com/user-attachments/assets/c926d836-a0af-4550-a317-92a9a035533a)

The site should look like this 

![image](https://github.com/user-attachments/assets/a0eb6c1c-4176-4546-bd49-9294abc8ce3b)



<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
