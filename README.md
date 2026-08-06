<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
After installing osTicket, the next step is to configure the help desk so it can properly manage users, agents, departments, permissions and ticket workflows. This ensures the ticketing system is organized, secure, and ready for production use.


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

  1. Configure system administrator
  2. Create and manage user Roles. 
  3. Establish departments.
  4. Configure support teams.
  5. Allow "anyone'to create tickets in Admin Panel.
  6. Configure Agents/ Workers.
  7. Configure Users/ Customers.
  8. Configure SLA
  9. Configure Help Topics for users to create tickets.


<h2>Configuration Steps</h2>

<p>
<img width="465" height="385" alt="image" src="https://github.com/user-attachments/assets/6fc46f64-c1cf-4f07-a4a0-4d2b61fb56b8" /> 

  The Admin/Analyst login page in which we use to log into osTicketing when we start administering and setting things up as a normal every day user.  
 
  <img width="852" height="538" alt="image" src="https://github.com/user-attachments/assets/69d6dcec-88bf-4db9-b35e-fe7434294e48" />


This is the end users osTicketing page where end users create their own tickets. The Admin Panel is used to configure the system, manage settings, create departments, assign permissions, and control the overall help desk environment.


<img width="967" height="386" alt="image" src="https://github.com/user-attachments/assets/cbc71375-5285-48fc-a7f5-69db9df1f146" />


I logged into the osTicket Admin Panel using the administrator account. On the welcome page, I clicked on "Admin Panel".


<img width="962" height="794" alt="image" src="https://github.com/user-attachments/assets/5f1079eb-6973-4c47-ba32-697b77112dea" />

On the Admin Panel page, clicked on "Agents" on the top right.

<img width="960" height="418" alt="image" src="https://github.com/user-attachments/assets/b2c04f17-a88a-4140-8360-37d063c79554" />

While on the Agents page, I clicked on "Roles". (The Role that will be created will be called "Supreme Admin". Supreme Admin  Role was created to provide full administrative access for managing the help desk, users, agents, departments, and system settings.)  


<img width="961" height="422" alt="image" src="https://github.com/user-attachments/assets/28743b19-b9e0-4759-b569-df033f0ef1c8" />

Roles determine what permissions each agent has inside osTicket. Click on "Expanded Access"


<img width="952" height="732" alt="image" src="https://github.com/user-attachments/assets/0b93ed79-a73a-4a69-ba3a-9131e6aa06dd" />

On the Expanded Access page click on "Permissions" we are now giving full permission to this agent. 


<img width="955" height="746" alt="image" src="https://github.com/user-attachments/assets/2b005dd1-cd3e-478b-b589-177eabf06891" />

On the Permissions page click on tickets, make sure all boxes have a blue check mark. then click on "Definition". 


<img width="955" height="603" alt="image" src="https://github.com/user-attachments/assets/fc6accad-2c39-4a3c-bb15-e784e564cdbf" />

After clicking on Definition, I named this Role: Supreme Admin. 


<img width="960" height="736" alt="image" src="https://github.com/user-attachments/assets/fa204c3e-ebca-4cc6-987a-7b2e31961af3" />


Click on "Permissions" again.

<img width="960" height="585" alt="image" src="https://github.com/user-attachments/assets/b403d857-5255-47e9-ac31-4917cb37e003" />


Click on "Tasks" and "Knowledgebase" make sure all the blue boxes are check marked. Once all boxes are checked click on "Add Role".


<img width="964" height="480" alt="image" src="https://github.com/user-attachments/assets/dbb42966-1373-4a6a-9c36-e93a2a19f88c" />

The Role has been successfully added for Supreme Admin. Now on to creating "Departments". (Admin Panel»Agents»Departments)


<img width="954" height="395" alt="image" src="https://github.com/user-attachments/assets/9ea318f8-80d1-4823-85a5-4164256b9592" />


Click on "Departments" which is right of Roles. ( Departments organize tickets based on the type of support being requested. I will create the SYSADMINS department to handle system administration issues. Departments also control which agents can view and work on specific tickets.) Click on "Add New Department" to proceed.

<img width="955" height="892" alt="image" src="https://github.com/user-attachments/assets/e65c5a3e-9350-4a17-af14-b762c08ad458" />

On the Add New Department page, under settings, for the Department Information I changed: Parent to Top-Level Department/ Name to SysAdminsDepart and the Outgoing Email noreply@yahoo.com.

<img width="954" height="905" alt="image" src="https://github.com/user-attachments/assets/42ec304c-9aa7-40ac-8aec-848eca999d07" />

I then clicked on "Create Dept" 


<img width="959" height="465" alt="image" src="https://github.com/user-attachments/assets/c4112f34-49e2-4d57-8e14-6830463b382d" />

The SysAdminsDepart was Successfully added.


<img width="956" height="374" alt="image" src="https://github.com/user-attachments/assets/ddc310d5-c74d-4e7c-b2ba-2ad4b30c17c6" />

Now I will configure "Teams". (Admin Panel»Agents»Teams) Teams allow agents from different departments to collaborate on the same tickets. Start by clicking on "Add New Team" on the Teams page.


<img width="957" height="707" alt="image" src="https://github.com/user-attachments/assets/99a36917-f1da-412e-8872-28277018cd2a" />

Under Team information, I named it "Online Banking". (I created the Online Banking team so agents with different specialties can work together to resolve customer issues efficiently.) Then I clicked "Create Team". The Teams where successfully created.

<img width="957" height="719" alt="image" src="https://github.com/user-attachments/assets/11b65419-4b7d-426c-9bb6-cbfaf0c23ac0" />

The next thing that I Configured was to allow anyone to create tickets. Admin Panel»Settings»User Settings page. Under the Authentication Settings, I unchecked the "require registration and login to create tickets", then clicked on the Save Changes button. (This was done only to allow anyone to create tickets for the sake of this project.)


<img width="953" height="354" alt="image" src="https://github.com/user-attachments/assets/d6fb5b7a-2b8e-4f9b-ae94-f388600bae3a" />

The next thing was to Configure Agents. ( Agents are employees who manage and resolve customer support tickets.  Admin Panel/Agents/Agents. I then clicked Add New Agent


<img width="951" height="748" alt="image" src="https://github.com/user-attachments/assets/b9133192-c870-48af-bb6f-74cff0db2c22" />


I created agent accounts and assigned each one to the appropriate department based on their responsibilities. Sally Smith (SysAdmin Department) & Bob Fox (Support Department).                                                                     Under Account on the Add New Agent [Name: Sally Smith/ Email Address: Sally@gmail.com/ Username: Sally]  


<img width="950" height="589" alt="image" src="https://github.com/user-attachments/assets/6e88264a-ec75-4369-8891-4e1c160c3ace" />

I continued and clicked Access to assign Sally Smith's Primary Department:                         Support/TopLevelDepartment & assigned her under Supreme Admin.


<img width="953" height="527" alt="image" src="https://github.com/user-attachments/assets/9c7f3a00-27f5-4ab9-95d1-ebea08795664" />

I proceeded to "Permissions" and checked all the boxes. I then proceeded to "Teams".


<img width="955" height="462" alt="image" src="https://github.com/user-attachments/assets/fb79f002-5ee8-46be-a299-0e64d367853e" />


Under Teams to assigned Sally Smith to the Online Banking Team. I then clicked the Yellow Create button.

<img width="953" height="255" alt="image" src="https://github.com/user-attachments/assets/ae11211f-6c6d-436e-a81f-b2e9d4178d62" />


Sally Smith was Successfully assigned and added. 

<img width="957" height="611" alt="image" src="https://github.com/user-attachments/assets/aea37162-9289-4f88-a6d6-554b3c0a3b52" />


I then assigned Bob Fox's role. Admin»Agents»Add New                                                                  Under Account Name: Bob Fox/ Email Address: bob@yahoo.com/ Username: Bob 


<img width="957" height="574" alt="image" src="https://github.com/user-attachments/assets/ce027d6f-3a9a-4dd8-8de7-6b6d54d7ee66" />


Next, I clicked "Access" Primary Department: Support and View Only for Bob's role.

<img width="972" height="531" alt="image" src="https://github.com/user-attachments/assets/a7aaece4-2b42-49b5-992a-c0fb2faea037" />

 
Checked all boxes Under Permissions (Users). 


<img width="831" height="472" alt="image" src="https://github.com/user-attachments/assets/7d2cdb60-c018-4b18-a553-696f0d891d64" />


Clicked Teams and left it as is, then proceeded to click the yellow Create button.

<img width="954" height="267" alt="image" src="https://github.com/user-attachments/assets/7502b3f1-a42f-47e8-a2e6-ec4fe2706332" />


Bob was Successfully Added.

<img width="953" height="424" alt="image" src="https://github.com/user-attachments/assets/57ed044d-a508-4240-853d-767239fdbd62" />


Agents Sally Smith and Bob Fox were successfully Active in their Roles.

<img width="641" height="387" alt="image" src="https://github.com/user-attachments/assets/4761f49e-385e-46a3-9d03-4fde09ebe8bc" />

Updated the password for both Sally Smith and Bob Fox [Password1] same for Both (only for purpose of this project.).


<img width="958" height="431" alt="image" src="https://github.com/user-attachments/assets/4d80b2f7-34c0-4349-b91e-6694b3b8e4ce" />


Next I Configured End Users. Users are the customers who submit support requests.                                      Users are Looked up/Created in Agent Panel» Users» Add New (only for the purpose of this project.)


<img width="650" height="399" alt="image" src="https://github.com/user-attachments/assets/0ea45c10-3aac-4b6d-97a9-fb649e1dabc6" />


I created Sandra as a sample user account to simulate real a customer and to test the ticket submission and support workflow. Email Address: Sandra@myspace.com / Full Name: Sandra. I then clicked Add User

<img width="959" height="392" alt="image" src="https://github.com/user-attachments/assets/68e644b3-6615-4701-b7a5-2e562091e46e" />

 Sandra Ticket was submitted. 


<img width="956" height="606" alt="image" src="https://github.com/user-attachments/assets/7941ff46-829e-4339-a287-6c4ad3fc02bf" />

I Configured SLA Plans in Admin Panel»Manage»SLA

<img width="961" height="364" alt="image" src="https://github.com/user-attachments/assets/50da83b0-2b3a-4d32-9c7e-7cb03baed269" />

I clicked, Add New SLA Plan. Service Level Agreements (SLAs) define how quickly support tickets should be addressed. Higher-priority issues receive faster response times, while low-priority issues follow standard business-hour schedules. {Sev-A  Grace Period 1 hour high priority, Schedule (24/7); Sev-B Grace Period 4 Hour mid-priority Schedule (24/7); Sev-C Grace Period 8 Hour, high-priority  Schedule (24/7). *Business Hours*}

 
<img width="945" height="630" alt="image" src="https://github.com/user-attachments/assets/981fd43e-3f09-43a7-8ea3-1d743cac25ee" />


  Created first SLA, Sev-A  Grace Period 1 hour high priority, Schedule (24/7), then clicked Add Plan.
 SLA Sev-A, example completed 


<img width="960" height="397" alt="image" src="https://github.com/user-attachments/assets/05068735-d623-44a8-84bb-a56246dd6a79" />


 SLA Sev-A, example completed  (continue adding Sev-B & Sev-C)


<img width="948" height="637" alt="image" src="https://github.com/user-attachments/assets/8886fa59-ba94-4dd1-b207-70a4022d12f6" />


Created second SLA, Sev-B Grace Period 4 Hour mid-priority Schedule (24/7), then clicked Add Plan.  

<img width="952" height="626" alt="image" src="https://github.com/user-attachments/assets/4d21876d-438c-488b-8f16-6b102dc7f3b2" />

Last SLA, Sev-C Grace Period 8 Hour, high-priority  Schedule (24/7). *Business Hours*}, then clicked Add Plan. 

<img width="946" height="597" alt="image" src="https://github.com/user-attachments/assets/4cec4c1a-069b-4ca1-817d-776dc669ce0b" />


<img width="885" height="611" alt="image" src="https://github.com/user-attachments/assets/341c2ef0-5673-4894-bf2c-2dac82296c74" />


<img width="949" height="604" alt="image" src="https://github.com/user-attachments/assets/2029fc15-632d-43fb-bf85-16083d7eb460" />


<img width="601" height="465" alt="image" src="https://github.com/user-attachments/assets/012018b0-336d-44a9-8c01-7b8df196ced9" />


<img width="823" height="598" alt="image" src="https://github.com/user-attachments/assets/45d7f5c3-fe43-41f0-b222-9a24d4e41b4e" />


<img width="960" height="637" alt="image" src="https://github.com/user-attachments/assets/f28be458-71de-44ee-8f30-d9b0f76a0a79" />







