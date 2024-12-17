<p align="center">
<img src="https://i.imgur.com/1ODW79g.png" height="80%" width="80%" alt="osTicket logo"/>
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
- Set up Agent and User/Customer profiles
- SLA (Service Level Agreements), make our personaized categories
- Create Help Topics for better communication

<h2>Detailed steps</h2>

<p>
<img src="https://i.imgur.com/OORsIs0.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>

<p>
<img src="https://i.imgur.com/9x1XBS4.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
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
<img src="https://i.imgur.com/M0mgoJY.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/IsVnvBa.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
To get there, first make sure you are now in the Admin Panel. To ensure this, check if it says "Agent Panel", on the top-right, as it always links to the panel that is currently not in use. Now navigate to Agents>Roles and you will see the different levels of access that can be asssigned to specific roles. When you click on one of them, e.g. "Limited Access", and click on "Permissions", there are many options of controlling what the different levels of access mean for your use case, with helpful explanations. Go back to the Roles menu and select "Add New Role". Give the Role a clear name. In my case, I called it "Admin Lead". Now select the permissions tab and  for this role we would like Access to everything, thus we will tick every box in "Tickets", "Tabs" and "Knowledgebase". Now just click on the Yellow button "Add Role" and the role is established. Now that we have our first Role, let's create a few departments.
</p>
<br />
<p>
<img src="https://i.imgur.com/2QALvW6.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>

Why do we need Departments? They are often there in order to ensure the ticket will show up for the correct department within a company. Let's assume there is a security issue within the network. To ensure effective and secure operations it is imperative that the Cybersecurity Dept. will see and respond to the ticket. Maybe the Manager would like to be able to see all tickets. You will be able to find find the Departments options right next to the Roles, Agents>Departments. Notice that the program has prepared a "Maintenance" and "Support" department already, which is quite useful. Select "Add New Department". Let's create the Administrator Department. First, we choose to make it a "Top Level Department", Choose your name, I used the name Admins for this. There are options for assigning SLA's and Schedules, etc. here, however, we first have to configure more parameters for this. As you can notice, there are many options to customize the department for many needs. I will choose that only the department itself will receive associated alerts and notices. For the auto-response email I will choose my fictional email I have created on setup. As you click on the Access tab, you will have the option to add specific Agents to the dept; however, we haven't established any so far, which we will soon. For the time being, we can select "Create Dept".
<p>
<img src="https://i.imgur.com/qvRH3RW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
Next up, let's create a few teams. You can imagine Teams as certain Departments that have to coordinate/work with each other in some way. Go to Agents>Teams>"Add New Team". I will name them "Threat response team" and "everyday issues". Later on, we will have the option to add a team lead. At this moment, select "Create Team". Now I suggest adding at least another team that makes sense for your purpose. With Teams set up, you can now enter the first Agents into your system.
</p>
<br />
<img src="https://i.imgur.com/o0EW2gc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/Q2CZrAq.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/tBn8CG8.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/XQszoPq.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
From the Agents Panel, you may select Agents. You will notice that the system has created a default Agent under your name. Go to "Add New" and you will be greeted with an account setup page similar to online portals you may have used before. For the purposes of this tutorial, we can keep agent details simple, adding names, for the email adress you will need a valid email format, however it will not be used in any way, and finally a fitting username. next to the username line, set the agent's password. Uncheck the box "send the agent[...]email" and you will be able to enter it. Also for the ease of this presentation, uncheck the lower box "require password change[...]". I highly suggest to write down the login info in a text document for later use. In the "Access" and "Teams" tabs you will be able to assign the previously customized departments, assign a role and add the agent to a team. For my first Agent, I have assigned all the high level admin access I had created earlier. After everything is taken care you click "create", you will see the profile at the Agents tab. Now, I will let you create a second Agent now with less access.
<p>
<img src="https://i.imgur.com/LKvigGd.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/nKmSsJG.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/w1NHKv4.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/eYt8jK3.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now it is time to create our first Users, which might also translate to customers. We will create two of them for this tutorial. We will now switch to the "Agent Panel" by clicking on the corresponding link at the top-right of the program. The initial test ticket can be safely deleted. Navigate to Users>Add User. All that si needed is an email address and a Name. After you have created your Users, return to the User directory and you will see all listed. Again, it is best to write down usernames for ease of use. That's all! We are close to the end of the configuration, let's configure our SLA's.
<p>
<img src="https://i.imgur.com/jfPo1ah.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/MeC68ws.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/uTo10y4.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>
<img src="https://i.imgur.com/qwGHMH8.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
Service Level Agreements (SLA) are important in efficently communicating the severity of an issue and to ensure that the most important issues are taken care of ASAP. In bigger companies it can be the case that important IT professionals are needed to be able to respond to high level issues 24/7 to ensure sensitive data is not lost to hackers for example. With many popular data breach cases, e.g. with Sony Pictures, this is very impotant nowadays.
You will have to return to the admin panel. Go to Manage>SLA and click "Add new SLA plan". Choose a name first, then a custom grace period (in hours). The higher the urgency, the lower the period, afterwards the schedule. For the first priority SLA, I will use a 24/7 schedule, as someone has to respond to the ticket immediately. For priority two, I chose a 24/5 schedule (not on weekends). Now create a final SLA for less urgent cases. As you return to the SLA tab, you can see them neatly listed together.
<p>
<img src="https://i.imgur.com/rIPQUai.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
For the last step, we set up Topics needed for the End-User. Everyone creating a ticket is then able to pick a Topic "category" to quickly let the Helpdesk know what type of issue is need of addressing. In the Admin Panel, go to Manage>Help Topics. Click on "Add New". Name the topic and select a "Parent Topic", which is a rough indicator of the User's issue. Tickets can be labeled as internal, which enables only agents to choose a certain topic if they personally open a new ticket. We can leave ours public at the moment. Create as many topics as you would like by clicking on "Add Topic" and then back on the "Help Topics" tab. After finishing your topics, you will see them in the "help topics" tab and you have the ability to move your own topics to the top for a more clear overview. Now we are finished with our initial configuration! After this setup, creating and working tickets will be a breeze, which is covered in my final osTicket segment.
As before, if using a cloud service like Azure, do make sure you stop the Virtual Machine on the portal to prevent more costs being incurred during your experimenting. Make sure your notes are saved as well and you will be able to use everything for the next segment.
