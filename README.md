# osticket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This demonstration outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br/>


<h2>Environments and Technologies Used</h2>

- Microsoft Azure Virtual Machine (VM)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- macOS

- Windows 10 Pro VM</b> (21H2)

<h2>List of Prerequisites</h2>

- Microsoft Azure 

- Microsoft Remote Desktop

- IIS Enabled

- PHP Manager: https://drive.google.com/file/d/1RHsNd4eWIOwaNpj3JW4vzzmzNUH86wY_/view?usp=share_link

- Rewrite Module: https://drive.google.com/file/d/1tIK9GZBKj1JyUP87eewxgdNqn9pZmVmY/view?usp=share_link

- PHP 7.3.8: https://drive.google.com/file/d/1snNMtLdCOpMtkCyD4mvl9yOOmvVIp9fP/view?usp=share_link

- Visual C++ Redistributable: https://drive.google.com/file/d/1s1OsGF3-ioO0_9LYizPRiVuIkb3lFJgH/view?usp=share_link

- MySQL: https://drive.google.com/file/d/1_OWh9p7VQLcrB0q_V7qT8yHl0xo5gv7z/view?usp=share_link

- osTicket: https://drive.google.com/file/d/1VeVXKlzHDRjeaVUL99ptq7qYbrbXdFxJ/view?usp=share_link

- HeidiSQL: https://docs.google.com/document/d/1WovrX2DaS9xkfaSr4LXyB4YnnWpXIgPCMMbbfgHmGVw/edit


<h2>Steps</h2>

<p>
1) <b>Create a vm on Microsoft Azure.</b><br/>
Within portal.azure.com, create a new VM by setting up a new resource group, username and password for admin configuration, selecting Windows 10 for an image and an option of 2 vcpus for a size, checking the checkbox for multi-tenant hosting licensing, clicking "Review + create", and to click "Create" after validation is passed.  
<img width="820" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/d10bf45d-4a48-4940-b048-4425162aeda6">
</p>
<br/>

<p>
2) <b>Access VM via remote desktop.</b><br/>
After the created vm is deployed, copy its public IP address and use it for Microsoft Remote Desktop and select to add a new pc. Access the vm by using the same username/password credentials used for setting up it up prior to deployment. 
<img width="1800" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/f9f311ce-eb00-4352-a39a-1e3889057de9">
<img width="602" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/a4c4b7dc-3705-4fec-ba02-05e9816ea1e1">
</p>
<br/>

<p>
3) <b>Enable IIS with the necessary configuration settings.</b><br/>
From now within the vm, go to Control Panel with the necessary directories. Ensure all checkboxes are checked within the Internet Information Services->World Wide Web Services->Common HTTP Features settings. Check the CGI checkbox within the Internet Information Services->World Wide Web 
Services->Application Development Features settings. Validate IIS was successfuly configured by performing a loopback with the 127.0.0.1 IP address in the search bar of Microsoft Edge.
<img width="1201" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/3e00da3d-2eda-4eb9-b304-115e1d1cfed6">
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/d4a5b553-ac66-4c37-bb1d-c90b49940aa8">
</p>
<br/>

<p>
4) <b>Install PHP Manager.</b><br/>
Copy the link URL for the PHP Manager and paste it on Microsoft Edge within the VM to download and install it afterwards.
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/47bfb5fc-0c86-486c-a760-44a65810ccfd">
</p>
<br/>

<p>
5) <b>Install Rewrite Module.</b><br/>
Copy the link URL for the Rewrite Module and paste it on Microsoft Edge within the VM to download and install it afterwards.
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/da4e2b23-6bfe-4964-891e-52baf68824ee">
<br/>

<p>
6) <b>Install PHP 7.3.8 and unzip its contents into C:\PHP.</b><br/>
Copy the link URL for PHP 7.3.8 and paste it on Microsoft Edge within the VM to download the zip file. Create a new folder called "PHP". In the "Downloads" file, two-finger tap the PHP 7.3.8 zip file, select "Extract all", and browse for the created "PHP" folder to extract within that folder.
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/3af68dd1-248f-40a5-8be2-fbdc65e4c58d">
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/520def2e-e9bb-4f27-8b3d-427e7ffbfff9">
</p>
<br/>

<p>
7) <b>Install Visual C++ Redistributable.</b>
Copy the link URL for Visual C++ Redistributable and paste it on Microsoft Edge within the VM to download and install it afterwards.
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/f3092b5d-5f9a-428e-8a23-cc4ff0119cfc">
</p>
<br/>

<p>
8) <b>Install MySQL.</b><br/>
Copy the link URL for MySQL and paste it on Microsoft Edge within the VM to download and install it afterwards. After the setup wizard is installed, select a standard configuration, type out a password for the "root" username, and click "Execute" when accessing the configuration wizard to finish setting up MySQL.
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/301234e5-cc9b-4a18-b2c4-f34494d75e26">
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/4d5ac152-2e84-473b-a352-1da16f97f187">
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/9bbff653-9318-454b-a01c-8fb8c67bb8ad">
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/f2c38a63-ad9a-4be1-912a-7ae51f5db8f0">
</p>
<br/>

<p>
9) <b>Open IIS to register new PHP version for the PHP Manager.</b><br/>
Search for IIS and ensure to run as an admin. Select PHP Manager when toggling the home menu and click "Register new PHP version". Browse C:\PHP and click on "php-cgi" to open it and run the new PHP version. Be sure to restart, stop, and start IIS in that order underneath "Manage Server" on the home menu.
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/283649e8-2d36-4387-b740-5ba6b5e2fc18">
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/42925388-5ebc-433a-991e-4417cfa05d27">
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/832ce282-0322-41c3-b9c8-ce79b9efca1d">
</p>
<br/>

<p>
10) <b>Install osTicket.</b><br/>
Copy the link URL for osTicket and paste it on Microsoft Edge within the VM to download and install it afterwards. Drag the "upload" folder from the osTicket zip file to Windows(C:)\inetpub\wwwroot and rename it as "osTicket".
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/6c92ffd5-eb72-4c6f-8848-7aa2c14dac2a">
</p>
<br/>

<p>
11) <b>Enable disabled features from the PHP Manager.</b><br/>
Click "Browse *:80 (http)" directly below Browse Folder on Sites->Default Web Site->osTicket below "Connections" on the home menu of IIS to be directed to osTicket Installer. While keeping the installer open, click on PHP Manager back on the home menu of IIS then click on "Enable or disable an extension" below "PHP Extensions" to be directed to that folder. Enable "php_imap.dll", "php_intl.dll", and "php_opcache" and refresh the tab for osTicket Installer to ensure the changes are configured.
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/172864b9-71f7-48e5-a8cb-8976475c9073">
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/83376ea7-2d58-413f-ae37-4c8f66e84983">
</p>
<br/>

<p>
12) <b>Rename configuration file and assign permissions.</b><br/>
On Windows(C:)\intetpub\wwwroot\osTicket\include, rename "ost-sampleconfig.php" to "ost.conifg.php"
Two-finger tap on "ost.config.php" to click on "Properities"-> "Security"->"Advanced"->"Disable inheritance". On the pop-up, click "Remove all inherited permissions from this object" then click "Apply"->"OK".
On "Security", click "Add..." and type "Everyone" for the object name and click "Check Names" to validate and then click "OK". Grant all permissions for "Everyone" then click 
"Apply"->"Ok".
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/0420f825-db06-4586-a2b5-2a24791cd59a">
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/3a44a3df-571b-4055-b81d-e9e988260b20">
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/7e761a38-d670-4ae4-9126-53108bdaa5ac">
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/d907e7e1-8c70-4393-b1d4-f27abab034de">
<br/>


<p>
13) <b>Fill out information to continue with osTicket installation.</b><br/>
Click "Continue" on the "osTicket Installer" tab. Fill out the information for "System Settings" and "Admin User". Use screenshot as possible reference for what to fill out. Leave "Database Settings" blank for now. 
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/149503df-25d8-4f70-a07e-f669d51f2c2e">
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/960b2534-3d80-4f0b-b146-c03c683992a3">
</p>
<br/>

<p>
14) <b>Install HeidiSQL.</b><br/>
Copy the link URL for HeidiSQL and paste it on Microsoft Edge within the VM to download and install it afterwards. Click "Skip" for next pop-up after installation. Click "New" and enter the password used earlier to set up the "root" username when configuring MySQL then click "Open".
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/6ff8619e-61bb-41a9-9c92-fa3dd3165c5e">
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/486bc241-6915-4df9-be75-7a6bf4279356">
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/d6bdd95a-acfd-4f19-8688-4deee8081a47">
</p>
<br/>

<p>
15) <b>Fill out the remaining information to finalize osTicket installation.</b><br/>
Back on the "osTicket Installer" tab, fill out the remaining information under "Database Settings" by typing the hostname and the same password for the "root" then click "Install Now". Ensure redirection to the right screen as shown in the screenshot.
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/97d6dc44-4e06-48e4-bd50-715f3f75c1f3">
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/299d442b-b63a-4d96-9c0e-c47e9f23e83e">
</p>
<br/>

<p>
16) <b>Perform various clean-up tasks.</b><br/>
Delete: Windows(C:)\intetpub\wwwroot\osTicket\setup and set permissions for "Everyone" to "Read" only.
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/955c6293-b09b-4312-be05-0f13becc7bfb">
<img width="1156" alt="image" src="https://github.com/XSimon2020/osticket-prereqs/assets/111246513/c7c30abc-4a51-485d-a8fc-622e0df966be">
</p>
<br/>

<b>This marks the end of the demonstration.<b>









    












