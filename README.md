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

- Microsoft Azure Account
- Remote Desktop Access
- IIS Basic Knowledge 
- osTicket Installation Files
- HeidiSQL

<h2>Installation Steps</h2>
<h3>1.) Create a Virtual Machine</h3>
<p>
In Microsoft Azure, create a VM and add it to a new Resource Group "osTicket"
</p>
  
  <b>.VM Name:</b> osticket-vm<br>
  <b>.Image:</b> Windows 10 Pro 22H2 - x64 Gen2<br>
  <b>.Size:</b> 2 vCPUs 16 GiB Memory

 Navigate to "Virtual Machines" page and select "Create" and choose "Azure virtual machine"

 ![image](https://github.com/user-attachments/assets/d860a194-f2ed-4263-a18c-8782ae083972)

 Create a new resource group and name the virtual machine, select the region and the image and operating system. 

 ![image](https://github.com/user-attachments/assets/0deb1e01-4e2f-453e-bb89-e96de3bad94c)

 Select the preferred cpu size, enter username and password, check the licensing box and review & create the VM. No need to change management, disks, or networking sections. 

 ![image](https://github.com/user-attachments/assets/31c034a4-2632-42cc-a478-c4e80f29f7d1)

<h3>2.) Log into Virtual Machine</h3>

Locate and copy the VM's Public's IP Address and using **Remote Desktop** (**or Windows App if using MacOS**) select "Add PC" and paste the IP Address in the PC Name tab, select add then use the username and password created during the VM setup to login.

![image](https://github.com/user-attachments/assets/6cf06f76-31b4-401e-b7ef-761725daefea)

<h3>3.) Download and Prepare Installation Files</h3>

Within the VM, download the osTicket-Installation-Files.zip and unzip it to your desktop. 

![image](https://github.com/user-attachments/assets/ac5a3263-22e0-42fa-a1c3-68e566983aff)

<h3>4.) Install IIS and Enable Required Features</h3>

Open Control Panel -> Programs -> Turn Windows features on or off. Install/enable IIS with the following features:

.World Wide Web Services -> Application Development Features -> [X] CGI

![image](https://github.com/user-attachments/assets/55ed1c92-fe4c-4ba3-a80d-893d46d20122)
![image](https://github.com/user-attachments/assets/c8d87fc1-a360-4ccb-954a-6a0435e29a76)

<h3>5.) Install Required Components</h3>

From the osTicket-Installation-Files folder:

.Install PHP Manager for IIS: PHPManagerForIIS_V1.5.0.msi.<br>
.Install Rewrite Module: rewrite_amd64_en-US.msi.<p>
![image](https://github.com/user-attachments/assets/4203b0e7-696a-4710-8763-d85f47a37856)

<h3>6.) Setup PHP</h3>

.Navigate to the C: drive and create the directory C:\PHP.<br>
.Unzip PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into the C:\PHP folder. <br>
.Install VC_redist.x86.exe.<br>
![image](https://github.com/user-attachments/assets/8a5c159e-6164-40bb-95ca-f420ce183a54)
![image](https://github.com/user-attachments/assets/ef310ea7-e9d5-4201-8ed8-3c2698fbbbbe)
![image](https://github.com/user-attachments/assets/fdac04a0-3297-432f-8412-e7edda9b0cc5)

<h3>7.) Install MySQL</h3>

.From the osTicket-Installation-Files folder, install MySQL 5.5.62 (mysql-5.5.62-win32.msi).<br>
.Select Typical Setup.<br>
.Launch the Configuration Wizard:<br>
.Standard Configuration<br>
.Input a username and password<br>

![image](https://github.com/user-attachments/assets/0ab4df84-0dc1-41b4-9982-b4dca38b868e)
![image](https://github.com/user-attachments/assets/4a0e5ab3-e718-4915-a1dd-f7dee7061818)
![image](https://github.com/user-attachments/assets/01507b87-3f43-4de6-8d2c-d908742bd1fb)
![image](https://github.com/user-attachments/assets/8d878a02-9558-4ac4-ac47-d2aed8c2868f)

<h3>8.) Configure IIS</h3>

.Open IIS as an administrator.<br>
.Register PHP:<br>
.Go to PHP Manager -> Register PHP path -> C:\PHP\php-cgi.exe.<br>
.Reload IIS (Stop and Start the server).<br>

![image](https://github.com/user-attachments/assets/16648a11-9ae1-4fd1-8c3d-6e7174211045)
![image](https://github.com/user-attachments/assets/32d6a4fb-b01c-4d36-82b1-b5a3842eb342)
![image](https://github.com/user-attachments/assets/2085a4c2-2021-4f21-86c0-2190777a2409)



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

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
