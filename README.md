# post-install-config
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket system
<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Agents
- Ticket properties
- Help topics
- SLA
- Departments
- Roles/permissions
- Users/Teams

![image](https://github.com/user-attachments/assets/0c0937a4-3647-4db9-b588-4956ed86fe90)![image](https://github.com/user-attachments/assets/4fa68515-3b69-4aee-b229-97f5e6f68d0b)

![image](https://github.com/user-attachments/assets/cdd8b1ff-74d5-46cd-a7fb-9350bf85a906)![image](https://github.com/user-attachments/assets/edc0e2be-dd48-44c6-abd6-30e00413d7d6)



1. Admin/Analyst Login Page

- URL: http://localhost/osTicket/scp/login.php

- This is where Admins and Analysts log in to manage everything behind the scenes in osTicket.

2. End-User Support Page

- URL: http://localhost/osTicket

- This is the page where users go to submit support tickets and check on their status.

3. Know the Difference: Agent Panel vs Admin Panel

- Agent Panel is for handling tickets—assigning them, responding, managing day-to-day stuff.

- Admin Panel is for the full setup—configurations, system settings, user permissions, etc.

4. Set Up Roles

- Path: Admin Panel > Agents > Roles

- Use this section to create different roles (like Supreme Admin, Agents, etc.) and assign what each role can and can’t do.

5. Set Up Departments

- Path: Admin Panel > Agents > Departments

- This is where you split up teams by department—like Help Desk, SysAdmins, or Networking—so tickets go to the right group and visibility is controlled.

6. Set Up Teams

- Path: Admin Panel > Agents > Teams

- Teams are helpful for grouping agents across departments. For example, you could create an “Online Banking” team using members from multiple departments.

7. Control Who Can Submit Tickets

- Path: Admin Panel > Settings > User Settings

- Uncheck the setting that allows unregistered users to create tickets.

- Enable “Require registration and login to create tickets” to make sure only registered users can submit..


![image](https://github.com/user-attachments/assets/7cb2a8f5-8505-43e1-9cfb-5dd02af78d3c)![image](https://github.com/user-attachments/assets/958655a8-1511-45f3-bb8e-aae898d7e256)
![image](https://github.com/user-attachments/assets/e381365e-16fc-4540-a748-558a36881708)![image](https://github.com/user-attachments/assets/305bef16-d6aa-4483-a84f-e40bb9dac4b3)

1. Add Agents (Your Team Members)

- Path: Admin Panel > Agents > Add New

- Add your team:

- Jane goes under the SysAdmins department

- John gets assigned to the Support department

2. Add Users (Your Customers)

- Path: Agent Panel > Users > Add New

- Add users like Karen and Ken as customers so they can start submitting tickets.

3. Set Up SLAs (Service Level Agreements)

- Path: Admin Panel > Manage > SLA

- Define your ticket response times:

- Sev-A: 1 hour grace period (24/7 support)

- Sev-B: 4 hour grace period (24/7 support)

- Sev-C: 8 hour grace period (Business Hours only)

4. Set Up Help Topics (What Users Pick When Submitting a Ticket)

- Path: Admin Panel > Manage > Help Topics

- Create categories users can choose from when they open a ticket:

- Business Critical Outage

- Personal Computer Issues

- Equipment Request

- Password Reset

- Other
