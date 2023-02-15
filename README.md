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

<h2>Prerequisites</h2>

- Resource Group
- Virtual Machine
- Remote Desktop Connection
- Internet Information Services (IIS)
- osTicket

<h2>Post-Install Configuration Objectives</h2>

- In this section we will create and configure osTicket environment.
- We will setup stuff as an admin.
- We will create role, department, team, agents and users.
- We will setup different SLA’s and create some help topics.

<h2>Configuration Steps</h2>
</p>
<p>
Login to the osTicket as an admin. Note that you can also switch between admin and agents panel by click to the top right corner of the screen.
</p>
<br />
<p>
<img src="https://i.imgur.com/ShJmDqO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Role is the permission granted to agents per department that they have access to. Each role has a set of permission that can be checked or unchecked for the agent given that role in association of the department that they have access to. In this case we will create a role called supreme admin and we will give people who have this supreme admin role to the access of everything.
  
  
Admin Panel -> Agents -> Roles
Add new role>Supreme admin
  

After adding a new role go to the permission and check all of the boxes, click task and check all of the boxes, click knowledgebase and check the box.

</p>
<br />

<p>
<img src="https://i.imgur.com/gL3PXY1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The ticket gets associated with the department and that specific department will takecare of that ticket.
  
  
Admin Panel -> Agents -> Departments
Add new department>System Administrator

</p>
<br />

<p>
<img src="https://i.imgur.com/X9CgYtn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  
The group of every department best members make one team.
  

Admin Panel -> Agents -> Teams
  
  
Level I Support
  
  
Level II Support
  
  
Add level II support and in members add yourself kanza in the team.


</p>
<br />

<p>
<img src="https://i.imgur.com/CBGcTRq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Admin Panel -> Settings -> User Settings
  
  
Registration Required: Require registration and login to create tickets 
  
  
</p>
<br />
<p>
<img src="https://i.imgur.com/tXl04pT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>



Agent is the person who solve the ticket.
  
Admin Panel -> Agents -> Add New
You can add anyone to the agent list by creating their user’s name, email, and password. In this case I added jane doe and john does as agents.
  
  
Jane Doe  
Access> Set to System Administrators>Set role to supreme admin>check permission>check teams and to level II support and create
  
  
John Doe 
Access>support>role set to view only>Extended Access set to support and create


</p>
<br />

<p>
<img src="https://i.imgur.com/uwwXNBM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

We can also add the End users. End user are the person who can create their own ticket.
  
  
Agent Panel -> Users -> Add New

Karen 
 

  
</p>
<br />

<p>
<img src="https://i.imgur.com/hgxaaOQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Add karen and ken to the end user.
</p>
<br />

<p>
<img src="https://i.imgur.com/TTGKh4f.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
SLA is the time frame on how long the ticket is going to open and then the help desk will be going to close the ticket.
  
  
Admin Panel -> Manage -> SLA


</p>
<br />
<p>
<img src="https://i.imgur.com/1GRonhI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Add these three SLA's
  
Sev-A (1 hour, 24/7)
  
  
Sev-B (4 hours, 24/7)

  
Sev-C (8 hours, business hours)
  
</p>
<br />

<p>
<img src="https://i.imgur.com/7yNI5Gi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
End user can choose the problem about what they are going to need help with, and to do this go to the
Admin Panel -> Manage -> Help Topics

  
Business Critical Outage

  
Personal Computer Issues

  
Equipment Request

  
Password Reset

</p>
<br />

<p>
