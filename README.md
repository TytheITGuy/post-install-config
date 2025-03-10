<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket: Post-Installation Configuration</h1>

<h2>Description</h2>
This project focuses on configuring osTicket, so it can be used properly as a ticketing system. It consists of setting up multiple agents along with their departments, roles, and permissions. As well as, configuring SLAs (Service Level Agreements), help topics, and users.<br/>
<br/>

This project is a continuation of the [osTicket: Prerequisites and Installation](https://github.com/TytheITGuy/osticket-prereqs) project.
<br />


<h2>Environments and Utilities Used</h2>

- <b>Microsoft Azure</b>
- <b>Virtual Machines</b>
- <b>Remote Desktop Connection</b>
- <b>osTicket</b>


<h2>Operating Systems Used </h2>

- <b>Windows 10</b>

<h2>Project Walk-through:</h2>

<p align="center">
To start configuring Roles Navigate to the "Agents" tab and click on "Roles" underneath the "Agents" tab. Enter a role name:

![01- Admin Panel - Roles](https://github.com/user-attachments/assets/84aaf0c7-583d-49ec-8117-5a51a02f02b7)

In the "Permissions" tab of this role, give this role all permissions in "Tickets", "Tasks", and "Knowledgebase". This will be our "Supreme Admin" Role: 

![02- Supreme Admin](https://github.com/user-attachments/assets/221adc34-8d52-4e1f-ae8a-6abc2a92cbca)

![03- Supreme Admin Permissions](https://github.com/user-attachments/assets/09c11a15-fd52-42ee-b92c-17aee4e95082)



To set up departments, while still in the "Agents" tab, click on "Departments" located just below the "Agents" tab. Name the department "System Administrators" and create the Department: 

![05-New Department](https://github.com/user-attachments/assets/8d815192-1d71-47df-b25f-f7de9f39504e)


Next, create a team by selecting the "Teams" tab, while still in the "Agents" tab. Then, name the team "Online Banking" and create team: 

![06- Adding a new team](https://github.com/user-attachments/assets/f4af0f5d-fbee-4fb8-896a-b8052b7f7f8a)


Now, to allow anyone to create tickets, go to the "Settings" Tab, and under "Authentication Settings" make sure that "Require registration and login to create tickets" is unchecked:  

![07- uncheck Registration](https://github.com/user-attachments/assets/10f9176a-a61f-4d92-8476-2901cf5deb4d)



To create agents (the help desk workers) navigate back to the "Agents" tab and select "Agents" and fill out the name, email, and username: 

![08-Creating users](https://github.com/user-attachments/assets/f3101db8-03d5-485d-8f91-ef2a955fccb5)


On the "Access" tab for this user select the "System Administrators" department and the "Supreme Admin" role created earlier: 

![09-Giving Jane access](https://github.com/user-attachments/assets/dd98b4a5-bc98-44ae-b41e-c6922eb0ddab)


Create one more agent as done previously, the only difference is in the "Access" tab select "Support" for the department:  

![10-John Agent](https://github.com/user-attachments/assets/1b3df76a-f906-439f-a406-3e49455e5aa5)


Next, to create a user (the customers) switch to the "Agent Panel" in orange in the top right> Users> Add User and put an email and name, then create. (I also made one more user with the same steps taken here): 

![11-Adding Customer](https://github.com/user-attachments/assets/17cb4775-0ad2-4d59-8d60-4908c2549648)


Configuring an SLA plan navigate back to Admin Panel> Manage> SLA create three SLAs with different severities, grace periods, and schedules like so:  

![12-Configuring SLA](https://github.com/user-attachments/assets/2c41d17e-fc1c-4507-8db2-605d213dc606)

![13- Sev A](https://github.com/user-attachments/assets/faa4aac4-e2e6-49cb-a611-81244c18647d)

![14-Sev B](https://github.com/user-attachments/assets/1cd1edb7-3b6d-4839-b665-05a3c4fa1147)

![15- Sev C](https://github.com/user-attachments/assets/92a1050b-87f0-4984-b569-477e8e600963)


Under the same "Manage" tab go to the "Help Topics" tab and create four help topics named, "Business Critical Outage", "Personal Computer Issues", "Equipment Request", and "Password Reset" all with the same settings like so:  

![16-Help Topics](https://github.com/user-attachments/assets/c14fdbbe-98d3-4d31-a7bb-198fff718936)



<h2>osTicket Setup Complete!</h2>

<b> We've successfully set up multiple agents along with their departments, roles, and permissions. As well as, configured SLAs (Service Level Agreements), help topics, and users! osTicket is now setup for the next project where I will create and work different tickets using multiple agents and users!  </b>
<br />
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
