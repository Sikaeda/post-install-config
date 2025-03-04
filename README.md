<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Setup post installation configuration for osTicket to prepare for help desk preparation.

<h2>Configuration Steps</h2>

<p>
Admin/Analyst Login Page:
http://localhost/osTicket/scp/login.php 

End Users osTicket URL:
http://localhost/osTicket 

Acknowledge Agent Panel vs Admin Panel

![image](https://github.com/user-attachments/assets/c959a912-21b0-40f7-9225-7f73d7cf2cd1)

![image](https://github.com/user-attachments/assets/de7a030a-d4f3-4322-a9ee-f05adda86d18)

(Note: the Admin Panel and Agent Panel in the top right corner are to navigate to those respective pages; NOT the name of the page you're currently on)

![image](https://github.com/user-attachments/assets/bf1a826e-8a21-44d8-86d8-5b57641cb073)

![image](https://github.com/user-attachments/assets/7a5c1278-5314-4d99-9390-2d463278dece)

![image](https://github.com/user-attachments/assets/19bce6f0-e61b-466f-8654-d56e9ac6002b)

Check every permission box in the "Ticket" "Tasks" and "Knowledgebase"

Configure Roles (for grouping permissions)
Admin Panel -> Agents -> Roles
Supreme Admin

![image](https://github.com/user-attachments/assets/f56bafca-1afc-4b3a-8a43-d0004f5b036d)

Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
Admin Panel -> Agents -> Departments
SysAdmins

![image](https://github.com/user-attachments/assets/6d5d40d9-4aaa-49b9-a00b-66fafab726c9)

Configure Teams
Admin Panel -> Agents -> Teams (Pull Agents from different Departments)
Online Banking

![image](https://github.com/user-attachments/assets/2088bde4-87f0-43bf-b8b0-04b61675d7dd)

Allow anyone to create tickets
Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)
Registration Required: Require registration and login to create tickets 

Configure Agents (workers)
Admin Panel -> Agents -> Add New
Jane (Dept: SysAdmins)
John (Dept: Support)

Configure Users (customers)
Agent Panel -> Users -> Add New
Karen
Ken

![image](https://github.com/user-attachments/assets/66f74ddc-c8f6-4610-97e0-29f085fa2755)

Configure SLA
Admin Panel -> Manage -> SLA
Sev-A (Grace Period: 1 hour, Schedule: 24/7)
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
Sev-C (Grace Period: 8 hours, Business Hours)

![image](https://github.com/user-attachments/assets/55ccf943-fa0e-4117-8f3b-0227e615737a)

Configure Help Topics (For when users create a ticket)
Admin Panel -> Manage -> Help Topics
Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset
Other


</p>
<br />
