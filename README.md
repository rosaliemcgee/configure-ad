<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Create 2 Virtual Machines in Azure; one with Windows 10(Client-1) and the other with Windows Server 2022(DC-1)
- Install Active Directory Domain Services
- Create an Administrator Account
- Create non-administrative users

<h2>Deployment and Configuration Steps</h2>
Created two Virtual Machines in Azure and logged into them with Remote Desktop connection.
<p>
<img src="https://i.imgur.com/21NrJPW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/VS56djC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/p8woKc2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

<p>
Installed Active Directory Domain Services in the Windows Server VM.
<img src="https://i.imgur.com/iPQsfLL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/KFHMjTt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

<p>
Created an administrative user for Jane Doe(jane_admin) and then made it a member of Domain Admins.
<img src="https://i.imgur.com/5UwbxMB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/WHPa1Yd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

<p>
Joined Client-1 to mydomain.com on DC-1 by changing Client-1 DNS settings in Azure and point it to the Domain Controller's private IP address on DC-1; also made Client-1 accessible by Remote Desktop so other non-admin users can login on the computer.
<img src="https://i.imgur.com/jeJr3s5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/vPEjFtc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

<p>
Generated some additional users with resources from class instructor. They were inserted into the _Employees Organizational Unit.
<img src="https://i.imgur.com/MbVGOw4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/CfCJ8WW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

<p>
Logged in as one of the generated user accounts.
<img src="https://i.imgur.com/GV587jf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />
