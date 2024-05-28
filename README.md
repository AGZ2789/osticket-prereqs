<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>
🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷
🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Enabled IIS (Internet information services)
- Install web platform installer 
- Install MySQL and set up the username and password
- Install C++ redistributable
- Configure permissions and install OS Ticket

<h2>Installation Steps</h2>

🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷

🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶

- <h3>Create Resource Group</h3>

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-12_19-54-58](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/d8dddb6c-57f0-41df-9898-d7659afc43cc)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-12_19-07-51](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/d2b708fe-2321-4d8c-b2f6-ba68360491a5)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-12_19-58-19](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/80cc3dc1-b6a3-4af9-a2b0-2a5d22f7e0b6)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-12_19-59-13](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/cb8625b6-31c9-4be0-952c-0ac39bd08055)




🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷
🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶

- <h3>Create Virtual Machine</h3>

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-12_19-54-10](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/deb24f47-9b0a-4587-8dd4-e118afa6036d)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-12_20-03-40](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/9cf234b8-93ca-4e6d-bb5c-ac34bc5f9686)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-12_20-14-13](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/6a092a9a-5bda-4146-a0f5-4121165e72e7)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_13-10-29](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/e7b7e502-c35c-45f9-b8ed-0bb5b29a045c)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_13-01-17](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/6dea61b0-4530-43e8-92e8-2532883515e8)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-12_20-19-39](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/185b0b09-4948-4e3f-9ba0-43add1bc530d)

🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷
🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶

- <h3>Microsoft remote Desktop</h3>

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-14_16-43-51](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/99c73f6c-43c8-410e-b2d5-2d1b9df2a668)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-14_16-47-27](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/312aa278-2eb7-4892-95cb-d477e0967040)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-14_16-48-48](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/2463d3ea-1832-48ff-a0f8-915d9281f615)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-14_16-50-30](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/75baa465-29d4-4e43-96f1-d62cd50ac52a)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-14_16-51-26](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/79a6adb3-b7d7-4810-a51d-79159c3f78f2)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-14_16-51-45](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/f6f2b87f-713d-4f80-84e4-c0d44922d7dc)


🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷
🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶

- <h3>Enable (IIS) Internet Information Services</h3>

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-14_18-52-44](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/94f56e21-fce4-49b5-b090-dbcca0b4cad5)


![Snipaste_2024-05-15_13-45-48](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/1cac7590-09ad-4171-aede-8e6598c85721)


🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷
🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶

- <h3>Download PHP Manager for IIS</h3>

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Screenshot 2024-05-02 131816](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/014ad36e-8db1-49d3-b5f1-cabf8375a9f7)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Screenshot 2024-05-02 131911](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/e565e7b8-6464-4b7e-905f-0258b2eb8b13)

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_13-52-03](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/8c33c02a-0dfc-4922-949d-82fcc2b6c40f)



🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷
🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶

- <h3>Download IIS URL Rewrite Module</h3>

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Screenshot 2024-05-02 132202](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/c59c0662-8096-47de-90d0-65f033409993)

![Screenshot 2024-05-02 135756](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/c3832229-f126-470a-9890-345c92b7c04e)


🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷🔷
🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶🔶

- <h3>Create Directory C:\PHP</h3>

🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻🔻

![Snipaste_2024-05-15_14-04-54](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/aa9e684e-f4af-4971-93f6-b0454dfde596)

![Snipaste_2024-05-15_14-12-05](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/e5cfc623-b0a8-4d62-9088-6d75ad5e4eb2)

![Snipaste_2024-05-15_14-13-59](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/9c645f9e-fde1-4800-b63b-86414cc74812)

- <h3>Download PHP 7.3.8 | Unzip contents into C:\PHP</h3>

![Snipaste_2024-05-15_14-28-44](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/0f36bd0d-d407-45c7-b975-c657713f2a04)

![Snipaste_2024-05-15_14-34-30](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/2faf8d18-4785-4805-aaee-ad0b133ac9c9)

![Snipaste_2024-05-15_15-02-55](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/26746735-c847-435f-9464-b0b0de0538cd)


- <h3>Download VC redist x86.exe | Microsoft Visual C++ 2015-2022 Redistributable (x86)</h3>

- <h3>MySQL 5.5.62</h3>

- <h3>Open IIS as Administrator</h3>

![Snipaste_2024-05-15_15-51-41](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/c9795f54-c4a4-4c79-a31a-346eabbab6d6)




- <h3>Install osTicket</h3>

![Snipaste_2024-05-15_15-57-10](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/49e899f9-5b59-4f61-9f16-02a01cdeb3f0)



- <h3>Rename ost-config.php</h3>

![Snipaste_2024-05-15_17-38-15](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/ef57f503-39a8-4204-bf2e-cfce82fa4378)





- <h3>Assign Permissions ost-config.php</h3>

![Snipaste_2024-05-15_17-39-58](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/88be153e-111a-4cfc-bbc4-cb9dd2ffe170)

![Snipaste_2024-05-15_18-34-06](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/a4a1f527-2f74-4775-85af-d740e2b4804d)

![Snipaste_2024-05-15_18-36-47](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/e5cebc98-ea44-41be-b7d5-9e6bc8cee1f3)

- <h3>Download & Install HeidiSQL</h3>

![Snipaste_2024-05-15_19-03-57](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/b6a5b8fa-b2ae-4ce9-8343-e3121fb32df0)

![Snipaste_2024-05-15_19-10-56](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/8439c9fe-4fcb-408b-8c5f-636c0350d76a)


- <h3></h3>




- <h3></h3>




- <h3></h3>




- <h3></h3>


![Snipaste_2024-05-15_19-56-43](https://github.com/AGZ2789/osticket-prereqs/assets/84995125/b674a1c2-430a-473a-b30c-21a39608aae9)





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

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br /># osticket-prereqs
