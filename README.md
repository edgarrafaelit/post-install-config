<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.
We'll be using the administrative end of osTicket to create a small Helpdesk team and some employees for them to help. We will configure Service Level Agreements (SLAs), assign permissions to our Helpdesk Team and create some topics to help our employees specify the domain of their IT issue.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents
- Configure Users
- Configure Help Topics
<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/j1axVMt.png" height="80%" width="80%" alt="osTicket Landing Page"/>
</p>
<p>
From the landing page we want to navigate to the admin panel on the top right of the screen.
</p>
<br />

<p>
<img src="https://i.imgur.com/FQ7wyCQ.png" height="80%" width="80%" alt="Navigating to the Roles tab"/>
</p>
<p>
From the admin panel we navigate to the "Agents" tab and find Roles.
</p>
<br />

<p>
<img src="https://i.imgur.com/WIS9BKn.png" height="80%" width="80%" alt="Creating a role called Supreme Admin"/>
</p>
<p>
We're creating a Role called "Supreme Admin" with all privileges.
</p>
<br />
</p>
<br />

<p>
<img src="https://i.imgur.com/AYhrTma.png" height="80%" width="80%" alt="Creating a Department called System Administrators"/>
</p>
<p>
Back under the "Agents" tab we find "Departments" and create a department called "System Administrators".
</p>
<br />

<p>
<img src="https://i.imgur.com/XRdVrcj.png" height="80%" width="80%" alt="Creating a Team called Level II SUpport"/>
</p>
<p>
One more under the "Agents" tab we find the "Teams" tab. We're creating a team called "Level II Support."
</p>
<br />

<p>
<img src="https://i.imgur.com/cxTqnPD.png" height="80%" width="80%" alt="Require registration and login to create tickets"/>
</p>
<p>
we want to allow anyone to create a ticket but we also want to require them to authenticate when they submit a new ticket. From the Admin Panel, we navigate to "Settings" then "User Settings" and click the box "Require registration and login to create tickets"
</p>

<p>
<img src="https://i.imgur.com/z2rQoDb.png" height="80%" width="80%" alt="creating agents"/>
</p>
<p>
We want to create two Agents that will make up the support team for our fake company. From the Admin panel navigate to "Agents" and click "Add New".
</p>
<br />

<p>
<img src="https://i.imgur.com/YtcQrS2.png" height="80%" width="80%" alt="Jane is a Supreme Admin"/>
</p>
<p>
Make sure to assign Access for your new agents. We're giving Jane the Supreme Admin in the System Administrators Team
</p>
<br />

<p>
<img src="https://i.imgur.com/c7Ywsd3.png" height="80%" width="80%" alt="John is a Support Team Member"/>
</p>
<p>
Our next Agent John will be a member of the Support Team with a Role of Expanded Access.
</p>
<br />

<p>
<img src="https://i.imgur.com/o5wqnlc.png" height="80%" width="80%" alt="A note on password creation"/>
</p>
<p>
Make note that when setting the password for these accounts we would normally require the employee to create a new password upon their next login. We might also send them an email with instructions on how to create their own password. For the purposes of this lab, we have decided to opt out of both.
</p>
<br />

<p>
<img src="https://i.imgur.com/SY1Olp5.png" height="80%" width="80%" alt="Creating Users"/>
</p>
<p>
Now we can create our users. Navigate to the "User Panel" on the top right hand side of the screen and find the "Users" tab. We'll be adding two new users.
</p>
<br />

<p>
<img src="https://i.imgur.com/GrQnvki.png" height="80%" width="80%" alt="Creating a User"/>
</p>
<p>
First we create our user.
</p>
<br />

<p>
<img src="https://i.imgur.com/wHvsZnK.png" height="80%" width="80%" alt="Registering User"/>
</p>
<p>
Then we register our user. Keep in mind that we would normally want to check the box that requires users to change their password upon login. Osticket also has an option to send an email to the user so that they can register their account themselves.
</p>
<br />

<p>
<img src="https://i.imgur.com/mEBZtlE.png" height="80%" width="80%" alt="Configuring Service Level Agreements"/>
</p>
<p>
Now we can configure Service Level Agreements for our fake company. In most instances an SLA can take the form of a variety of separate policies that support team members adhere to. In the case of OsTicket, we'll be configuring a general rule of how long it should take for each ticket to be resolved.
</p>
<br />

<p>
<img src="https://i.imgur.com/4q4RPZ1.png" height="80%" width="80%" alt="Sev-A"/>
</p>
<p>
For Sev-A, we'll set the SLA to have a 1 hour window 24/7. Maybe this is for a security company or for an important e-commerce website.
</p>
<br />

<p>
<img src="https://i.imgur.com/dI8DxWS.png" height="80%" width="80%" alt="I doon't have a good example for this SLA"/>
</p>
<p>
For Sev-B, we'll set the SLA to have a 4 hour window 24/7.
</p>
<br />

<p>
<img src="https://i.imgur.com/yca9cE8.png" height="80%" width="80%" alt="Sev-C"/>
</p>
<p>
For Sev-B, we'll set the SLA to be an 8 hour time window within business hours. This is for more mundane issues like a mouse not working or maybe a dead pixel on an employee's monitor.
</p>
<br />

<p>
<img src="https://i.imgur.com/OHXEbtX.png" height="80%" width="80%" alt="Help Topics topic"/>
</p>
<p>
Now we're ready to assign Help Topics that allow Users to specify the domain of their ticket request and help Agents in organizing the severity of said tickets.
</p>
<br />

<p>
<img src="https://i.imgur.com/NlhVNkK.png" height="80%" width="80%" alt="Look at all those tops!"/>
</p>
<p>
In the next lab we'll be creating tickets through our user accounts and assigning them to Agents.
