<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-Premise Active Directory Deployed using Azure Virtual Machines </h1>
For this project, I deployed two virtual machines using Microsoft Azure: one hosting a Windows Server image, and the other hosting a Windows 11 Pro image. The VMs were configured into a Virtual Network and the network settings were configured in order for them to work in unison. I then created 50 users/employees using PowerShell to simulate a small business, as far as numer of users. Finally, I setup Windows Server as a Domain Controller, created and admin user, and did some trouble shooting for a "user" having sign on issues.

<h2>Technology Used</h2>

- Microsoft Azure: Virtual Machines & Compute
- Active Directory Domain Services 
- Remote Desktop
- Powershell

<h2>Operating Systems Used</h2>

- Windows Server 2022
- Windows 11 Pro

<h2>Deployment Steps:</h2>

<h2>Step 1) Successfully provisioned a Resource Group containing the lab's VNet and two VMs</h2>

<img width="1916" height="1052" alt="Successfully Deployed DC-Client VMs" src="https://github.com/user-attachments/assets/1e73ebfa-050c-446d-9ba1-a002b5f79ff1" />

<h2>Step 2) Reconfigured the Domain Controller's NIC Private IP to "static"</h2>
<img width="1917" height="928" alt="DC1 Static IP" src="https://github.com/user-attachments/assets/430ab581-2c93-4a34-b8c4-6c4bd3739834" />

<h2>Step 3) Reconfigured Client-1's DNS settings to DC-1's Private IP Address</h2>
<img width="1853" height="1092" alt="Client1 DNS to DC1 Private Ip" src="https://github.com/user-attachments/assets/5d78fd5c-9556-4e89-9def-18c798ec1cc6" />

<h2>Step 4) Successful Windows Server Connection using RDP - Deployment of Active Directory Domain Services - Creation of Organizational Units - Created "Users/Employees" using PowerShell</h2>
<img width="1888" height="1192" alt="Successful DC Connection" src="https://github.com/user-attachments/assets/eabe2aa3-3540-4c2e-9c11-354e307c4357" />
<img width="1887" height="1181" alt="Created  employees  using Python Script" src="https://github.com/user-attachments/assets/8a082ff9-3fe5-4a95-8d0f-c1c5e6c626df" />

<h2>Step 5) Configured a Custom User Lock Out Policy</h2>
<img width="1881" height="1198" alt="Custom Lock Out Policy in Group Policy Management Console" src="https://github.com/user-attachments/assets/c03dc8eb-87bf-4d0e-9469-f40628968d0d" />

<h2>Step 6) Chose a Random "Employee" to Simulate an Account Lockout</h2>
<img width="780" height="577" alt="Account Lockout Message" src="https://github.com/user-attachments/assets/3fab1411-dfc6-4e4f-94dd-3b63668d474a" />

<h2>Step 7) Unlocked User's Account and Reset Password</h2>
<img width="1846" height="1089" alt="User Account Unlocked and Password Reset" src="https://github.com/user-attachments/assets/5712732b-8bb2-4515-8674-d21ae8507767" />

<h2> Step 8) Successfully Logged into User's Account after Reset using Client-1 VM </h2>

<img width="833" height="836" alt="Successful Login after Reset" src="https://github.com/user-attachments/assets/4a7e498c-8cd3-4315-8dae-a8436f3bebe8" />

<h2>End) The Resource Group and all of its Resources were Deleted upon Completion of this Project *Not Pictured*</h2>










