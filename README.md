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
To start, log in using your osTicket admin username and password. The first thing of note here is the two different panels that can be accessed, the "Admin Panel", as well as the "Agent Panel", which, as an Admin you will be able to switch by clicking on the corresponing panel name in the top right of the window. In the Admin Panel you will be able to make many changes on the backend, which will be used for the most part in this guide. Whereas the Agent Panel is used for actively managing tickets and where a lot of time is spent as a Helpdesk Agent. Now it is time to begin with our first step in our configuration, the Roles.
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
To get there, first make sure you are now in the Admin Panel. To ensure this, check if it says "Agent Panel", on the top-right, as it always links to the panel that is currently not in use. Now navigate to Agents>Roles and you will see the different levels of access that can be asssigned to specific roles. When you click on one of them, e.g. "Limited Access", and click on "Permissions", there are many options of controlling what the different levels of access mean for your use case, with helpful explanations. Go back to the Roles menu and select "Add New Role". Give the Role a clear name. In my case, I called it "Admin Lead". Now select the permissions tab and  for this role we would like Access to everything, thus we will tick every box in "Tickets", "Tabs" and "Knowledgebase". Now just click on the Yellow button "Add Role" and the role is established. 
</p>
<br />
<p>
<img src="https://i.imgur.com/IsVnvBa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/IsVnvBa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
