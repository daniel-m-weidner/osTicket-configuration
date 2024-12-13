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

<h2>Steps to configure osTicket after initial setup</h2>

- Establish Roles, as well as:
- Departments
- Teams
- Establish ticket creation rules: registration requirement
- Set up Agent and User/Customer profiles
- SLA (Service Level Agreements), make our personaized categories
- Create Help Topics for better communication

<h2>Detailed steps</h2>

<p>
<img src="https://i.imgur.com/OORsIs0.png" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>

<p>
<img src="https://i.imgur.com/9x1XBS4.png" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/3HC2WtT.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
To start, log in using your osTicket admin username and password. The first thing of note here is the two different panels that can be accessed, the "Admin Panel", as well as the "Agent Panel", which, as an Admin you will be able to switch by clicking on the corresponding panel name in the top right of the window. In the Admin Panel you will be able to make many changes on the backend, which will be used for the most part in this guide. Whereas the Agent Panel is used for actively managing tickets and where a lot of time is spent as a Helpdesk Agent. Now it is time to begin with our first step in our configuration, the Roles. These are important to ensure that every "Role" which utilizes the system only has access to what is neccessary for them, e.g the accounting department usually does not need to be able to update tickets, however might need to view the active tickets sometimes.
</p>
<br />

<p>
<img src="https://i.imgur.com/M0mgoJY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/IsVnvBa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To get there, first make sure you are now in the Admin Panel. To ensure this, check if it says "Agent Panel", on the top-right, as it always links to the panel that is currently not in use. Now navigate to Agents>Roles and you will see the different levels of access that can be asssigned to specific roles. When you click on one of them, e.g. "Limited Access", and click on "Permissions", there are many options of controlling what the different levels of access mean for your use case, with helpful explanations. Go back to the Roles menu and select "Add New Role". Give the Role a clear name. In my case, I called it "Admin Lead". Now select the permissions tab and  for this role we would like Access to everything, thus we will tick every box in "Tickets", "Tabs" and "Knowledgebase". Now just click on the Yellow button "Add Role" and the role is established. Now that we have our first Role, let's create a few departments.
</p>
<br />
<p>
<img src="https://i.imgur.com/2QALvW6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Why do we need Departments? They are often there in order to ensure the ticket will show up for the correct department within a company. Let's assume there is a security issue within the network. To ensure effective and secure operations it is imperative that the Cybersecurity Dept. will see and respond to the ticket. Maybe the Manager would like to be able to see all tickets. You will be able to find find the Departments options right next to the Roles, Agents>Departments. Notice that the program has prepared a "Maintenance" and "Support" department already, which is quite useful. Select "Add New Department". Let's create the Administrator Department. First, we choose to make it a "Top Level Department", Choose your name, I used the name Admins for this. There are options for assigning SLA's and Schedules, etc. here, however, we first have to configure more parameters for this. As you can notice, there are many options to customize the department for many needs. I will choose that only the department itself will receive associated alerts and notices. For the auto-response email I will choose my fictional email I have created on setup. As you click on the Access tab, you will have the option to add specific Agents to the dept; however, we haven't established any so far, which we will soon. For the time being, we can select "Create Dept".
<p>
<img src="https://i.imgur.com/IsVnvBa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/IsVnvBa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next up, let's create a few teams. You can imagine Teams as certain Departments that have to coordinate/work with each other in some way. Go to Agents>Teams.
