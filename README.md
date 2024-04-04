# osticket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This demonstration outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure Virtual Machine (VM)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- macOS

- Windows 10 VM</b> (21H2)

<h2>List of Prerequisites</h2>

- Microsoft Azure VM

- Microsoft Remote Desktop

- IIS Enabled

- PHP Manager: https://drive.google.com/file/d/1RHsNd4eWIOwaNpj3JW4vzzmzNUH86wY_/view?usp=share_link

- Rewrite Module: https://drive.google.com/file/d/1tIK9GZBKj1JyUP87eewxgdNqn9pZmVmY/view?usp=share_link

- PHP 7.3.8: https://drive.google.com/file/d/1snNMtLdCOpMtkCyD4mvl9yOOmvVIp9fP/view?usp=share_link

- Visual C++ Redistributable: https://drive.google.com/file/d/1s1OsGF3-ioO0_9LYizPRiVuIkb3lFJgH/view?usp=share_link

- MySQL: https://drive.google.com/file/d/1_OWh9p7VQLcrB0q_V7qT8yHl0xo5gv7z/view?usp=share_link

- HeidiSQL: https://docs.google.com/document/d/1WovrX2DaS9xkfaSr4LXyB4YnnWpXIgPCMMbbfgHmGVw/edit

- Helpdesk Login (Within VM): http://localhost/osTicket/scp/login.php

- End user Login (Within VM): http://localhost/osTicket/

<h2>Installation Steps</h2>

<p>
1) Create a VM on Microsoft Azure
<img width="820" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/d10bf45d-4a48-4940-b048-4425162aeda6">
</p>
Within portal.azure.com, create a new VM by setting up a new resource group, username and password for admin configuration, selecting Windows 10 for an image and an option of 2 vcpus for a size, checking the checkbox for multi-tenant hosting licensing, clicking "Review + create", and to click "Create" after validation is passed.  
<p>
<br />

<p>
2) Access VM via remote desktop
<img width="1800" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/f9f311ce-eb00-4352-a39a-1e3889057de9">
<img width="602" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/a4c4b7dc-3705-4fec-ba02-05e9816ea1e1">
</p>
<p>
After the created vm is deployed, copy its public ip address and use it for Microsoft Remote Desktop and select to add a new pc. Access the vm by using the same username/password credentials used for setting up it up prior to deployment. 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
