<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket: Post-Installation Configuration</h1>
In this tutorial I will be showing you the Post-Installation steps you should take in order to configure OsTicket. We will create Agents, Users, Teams, Departments and SLA, in order to learn the capabilities of OsTicket. <br />



<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

<ul>
<li>Microsoft Azure (Virtual Machines/Compute)</li>
<li>Remote Desktop</li>
</ul> 

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Installed OsTicket

<h2>Configuration Steps</h2>
<h4>Step 1</h4>
<p>
  <ul>
    <li>Log into your virtual machine and <a href="http://localhost/osTicket/scp/login.php">OsTicket</a> </li>
    </ul> 
</p>
<br />

![image](https://github.com/cardosoguisilva/post-install-config/assets/157248613/765f6c3b-557e-4e7e-b958-1641c62ac118)

<h4>Step 2</h4>
<p>
  <ol type= "1">
    <li> - Configuring agent roles https://docs.osticket.com/en/latest/Admin/Agents/Roles.html
    - Go to Admin Panel -> Agents -> Roles, make yourself "Supreme Admin" by selecting all boxes in Tickets, Tasks and Knowlegdebase.
  
  ![image](https://github.com/cardosoguisilva/post-install-config/assets/157248613/8ce94b43-2a8d-40aa-b9fb-c2400b60ee7d)
    


- configuring departments https://docs.osticket.com/en/latest/Admin/Agents/Departments.html
- go to Admin Panel -> Agents -> Departments and create a new department called System ADM with system default.

![image](https://github.com/cardosoguisilva/post-install-config/assets/157248613/ce0ba838-c872-4675-b42d-546728800e3f)


- configuring teams https://docs.osticket.com/en/latest/Admin/Agents/Teams.html
- go to Admin Panel -> Agents -> Teams and create a new team " LEVEL II Support"

![image](https://github.com/cardosoguisilva/post-install-config/assets/157248613/d779666d-8b9c-4c2a-99cb-bebd81332ef3)


- now we're going to allow anyone to create a ticket.
- Admin Panel -> Settings -> User
- by default "Registration Required: Require registration and login to create tickets" should be unchecked. This will allow people to make ticekts anonymously 

![image](https://github.com/cardosoguisilva/post-install-config/assets/157248613/50b00f10-eff0-4da2-974c-eb0506641556)

- Now to create Agents https://docs.osticket.com/en/latest/Admin/Agents/Agents.html
-  Admin Panel -> Agents -> Add New add multiple agents create a username and password for each agent, write it down in case you forget. 
![image](https://github.com/cardosoguisilva/post-install-config/assets/157248613/15fe89c2-435b-48e1-9297-ed0da6c0a90d)
- unselect "Send the agent a password reset email" and  "Require password change at next login"
![image](https://github.com/cardosoguisilva/post-install-config/assets/157248613/c3ea4f16-68bb-44d5-971a-324673ca8790)
- make sure to select Access/Permissions/Teams for each agent.

- Configure Users https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html
- Click on Agent Panel -> Users -> Add New create two users.
![image](https://github.com/cardosoguisilva/post-install-config/assets/157248613/b4b97d75-00e6-4ab9-9eb4-bb346924ab63)

- Configure SLA https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html
- Admin Panel -> Manage -> SLA -> Add New SLA Plan
-Sev-A (1 hour, 24/7)
Sev-B (4 hours, 24/7)
Sev-C (8 hours, business hours) 
![image](https://github.com/cardosoguisilva/post-install-config/assets/157248613/33eb5d63-e335-4f84-94cd-9d977a1d35bf)

- Configure Help Topics https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html
- Admin Panel -> Manage -> Help Topics
- Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset

![image](https://github.com/cardosoguisilva/post-install-config/assets/157248613/996c8f99-b1b4-409a-88a7-e21f4e33cf2d)


    </li>
    </ol>
 
</p>



