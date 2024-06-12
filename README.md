<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

![](https://i.imgur.com/waxVImv.png)


<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

- [<b>Simple List</b>](https://docs.google.com/document/d/1JfsM1LRBu6UfCGy1wkADmG3cRzhmuzEoTLt9BRisgQ4/edit?usp=sharing)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used</h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Enabled IIS (Internet information services)
- Install web platform installer 
- Install MySQL and set up the username and password
- Install C++ redistributable
- Configure permissions and install OS Ticket

<h2>Installation Steps</h2>

![](https://i.imgur.com/waxVImv.png)

- <h3>Create a Resource Group in Azure</h3>

  - Name it RG-osTicket (or whatever you choose)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-12_19-54-58](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/d8dddb6c-57f0-41df-9898-d7659afc43cc)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-12_19-07-51](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/d2b708fe-2321-4d8c-b2f6-ba68360491a5)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-12_19-58-19](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/80cc3dc1-b6a3-4af9-a2b0-2a5d22f7e0b6)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-12_19-59-13](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/cb8625b6-31c9-4be0-952c-0ac39bd08055)


![](https://i.imgur.com/waxVImv.png)


- <h3>Create an Azure Virtual Machine</h3>
  
  - Create an Azure Virtual Machine using Windows 10, 4 vCPUs
  - Name: VM-osticket
  - Username: Labuser (or whatever you choose)
  - Password: Password1! (or whatever you choose)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-12_19-54-10](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/deb24f47-9b0a-4587-8dd4-e118afa6036d)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-12_20-03-40](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/9cf234b8-93ca-4e6d-bb5c-ac34bc5f9686)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-12_20-14-13](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/6a092a9a-5bda-4146-a0f5-4121165e72e7)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_13-10-29](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/e7b7e502-c35c-45f9-b8ed-0bb5b29a045c)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

- <h3>When creating the VM, It will create a new Virtual Network (Vnet)</h3>

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_13-01-17](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/6dea61b0-4530-43e8-92e8-2532883515e8)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-12_20-19-39](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/185b0b09-4948-4e3f-9ba0-43add1bc530d)

![](https://i.imgur.com/waxVImv.png)

- <h3>Open Microsoft Remote Desktop</h3>

  - Copy and paste Public IP Address from the Virtual Machine onto the Microsoft Remote Desktop Connection window
  
🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-14_16-43-51](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/99c73f6c-43c8-410e-b2d5-2d1b9df2a668)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

- Enter Credentials from the "Create a Virtual Machine" step, under Administrator Account

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-14_16-47-27](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/312aa278-2eb7-4892-95cb-d477e0967040)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-14_16-48-48](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/2463d3ea-1832-48ff-a0f8-915d9281f615)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-14_16-50-30](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/75baa465-29d4-4e43-96f1-d62cd50ac52a)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-14_16-51-26](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/79a6adb3-b7d7-4810-a51d-79159c3f78f2)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-14_16-51-45](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/f6f2b87f-713d-4f80-84e4-c0d44922d7dc)


![](https://i.imgur.com/waxVImv.png)

- <h3>Enable (IIS) Internet Information Services</h3>
- Install / Enable IIS in Windows with CGI and Common HTTP Features:
  - Open Run command —> Ctrl + R —> enter and open “control panel”
  - Navigate to Control Panel -> Programs -> Programs & Features.
  - Select "Turn Windows features on or off".
  - Ensure the following features are selected & enabled:
    - (IIS) Internet Information Services
    - Expand World Wide Web Services and select:
    - CGI
    - All Common HTTP Features

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-14_18-52-44](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/94f56e21-fce4-49b5-b090-dbcca0b4cad5)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

- Confirm installation by accessing http://127.0.0.1 in the browser.
  - Installation confirmation - Enter 127.0.0.1 (Local Host or the Loop Back)
on VM browser address bar —> press enter and the default IIS website should appear.
Note: 127.0.0.1 (Local Host or the Loop Back) = Meaning try to load a webpage that’s running off myself.

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_13-45-48](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/1cac7590-09ad-4171-aede-8e6598c85721)


![](https://i.imgur.com/waxVImv.png)


- <h3>Download PHP Manager for IIS from the Installation Files</h3>

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Screenshot 2024-05-02 131816](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/014ad36e-8db1-49d3-b5f1-cabf8375a9f7)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Screenshot 2024-05-02 131911](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/e565e7b8-6464-4b7e-905f-0258b2eb8b13)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_13-52-03](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/8c33c02a-0dfc-4922-949d-82fcc2b6c40f)



![](https://i.imgur.com/waxVImv.png)


- <h3>Download IIS URL Rewrite Module from the Installation Files</h3>

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Screenshot 2024-05-02 132202](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/c59c0662-8096-47de-90d0-65f033409993)

![Screenshot 2024-05-02 135756](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/c3832229-f126-470a-9890-345c92b7c04e)


![](https://i.imgur.com/waxVImv.png)


- <h3>Create Directory C:\PHP</h3>

  - Open File Explorer
  - Go to This PC --> Windows(C:) Drive --> Right click --> New --> Folder --> Name it "PHP"
  
🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_14-12-05](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/e5cfc623-b0a8-4d62-9088-6d75ad5e4eb2)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_14-13-59](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/9c645f9e-fde1-4800-b63b-86414cc74812)


![](https://i.imgur.com/waxVImv.png)


- <h3>Download PHP 7.3.8 from the Installation Files</h3>

  - Unzip contents into C:\PHP

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_14-28-44](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/0f36bd0d-d407-45c7-b975-c657713f2a04)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_14-34-30](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/2faf8d18-4785-4805-aaee-ad0b133ac9c9)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_15-02-55](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/26746735-c847-435f-9464-b0b0de0538cd)

![](https://i.imgur.com/waxVImv.png)

- <h3>Download VC redist x86.exe | Microsoft Visual C++ 2015-2022 Redistributable (x86) from the Installation Files</h3>

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Screenshot 2024-05-02 133812](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/4a45f7c5-3a64-4cb9-a678-5637e4ea4d93)

![](https://i.imgur.com/waxVImv.png)

- <h3>Download MySQL 5.5.62 from the Installation Files</h3>

  - Download MySQL 5.5.62 and follow steps 1-4 on the screenshot below
  
  - From the Installation Files, download and install MySQL 5.5.62 (mysql-5.5.62-win32.msi)
    - Typical Setup ->
    - Launch Configuration Wizard (after install) ->
    - Standard Configuration ->
    - Password1
  
🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-17_20-36-39](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/d9a5c2c4-aac9-4a19-a818-412ee41a9a91)

![](https://i.imgur.com/waxVImv.png)

- <h3>Open IIS as Administrator</h3>

- Go to sites -> Default -> osTicket
  - On the right, click “Browse *:80”
- Reload IIS (Open IIS, Stop and Start the server)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_15-51-41](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/c9795f54-c4a4-4c79-a31a-346eabbab6d6)

![](https://i.imgur.com/waxVImv.png)

- <h3>Install osTicket from the Installation Files</h3>

- Note that some extensions are not enabled

- Go back to IIS, sites -> Default -> osTicket
  - Double-click PHP Manager
  - Click “Enable or disable an extension”
    - Enable: php_imap.dll
    - Enable: php_intl.dll
    - Enable: php_opcache.dll
- Refresh the osTicket site in your browse, observe the changes

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_15-57-10](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/49e899f9-5b59-4f61-9f16-02a01cdeb3f0)

![](https://i.imgur.com/waxVImv.png)

- <h3>Rename ost-config.php</h3>

  - From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
  - To: C:\inetpub\wwwroot\osTicket\include\ost-config.php

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_17-38-15](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/ef57f503-39a8-4204-bf2e-cfce82fa4378)

![](https://i.imgur.com/waxVImv.png)

- <h3>Assign Permissions ost-config.php</h3>

  - Disable inheritance -> Remove All
  - New Permissions -> Everyone -> All

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_17-39-58](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/88be153e-111a-4cfc-bbc4-cb9dd2ffe170)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_18-34-06](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/a4a1f527-2f74-4775-85af-d740e2b4804d)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_18-36-47](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/e5cebc98-ea44-41be-b7d5-9e6bc8cee1f3)

![](https://i.imgur.com/waxVImv.png)

- <h3>Download & Install HeidiSQL</h3>

- Continue Setting up osTicket in the browser (click Continue)
  - Name Helpdesk
  - Default email (receives email from customers)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_19-03-57](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/b6a5b8fa-b2ae-4ce9-8343-e3121fb32df0)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

- From the Installation Files, download and install HeidiSQL.
  - Open Heidi SQL
  - Create a new session, root/Password1
  - Connect to the session
  - Create a database called “osTicket”

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_19-10-56](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/8439c9fe-4fcb-408b-8c5f-636c0350d76a)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

- Continue Setting up osticket in the browser
  - MySQL Database: osTicket
  - MySQL Username: root
  - MySQL Password: Password1
  - Click “Install Now!”

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_19-03-57](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/b6a5b8fa-b2ae-4ce9-8343-e3121fb32df0)


![](https://i.imgur.com/waxVImv.png)


- <h3>Congratulations, hopefully it is installed with no errors!</h3>
  
  - Browse to your help desk login page: http://localhost/osTicket/scp/login.php

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_19-56-43](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/b674a1c2-430a-473a-b30c-21a39608aae9)

![](https://i.imgur.com/waxVImv.png)

- <h3>End Users osTicket URL:</h3>

  - http://localhost/osTicket/

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-17_21-58-45](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/f10a7951-a771-49ad-b3ac-73388cc19f9a)

![](https://i.imgur.com/waxVImv.png)

- <h3>Clean up</h3>

  - Delete: C:\inetpub\wwwroot\osTicket\setup
  - Set Permissions to “Read” only: C:\inetpub\wwwroot\osTicket\include\ost-config.php

- Notes:

  - Browse to your help desk login page: http://localhost/osTicket/scp/login.php  
  - End Users osTicket URL: http://localhost/osTicket/
 
![](https://i.imgur.com/waxVImv.png)

