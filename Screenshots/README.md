Step 1. Active Directory Setup
•	Install Active Directory Domain Services
•	Promoted server to Domain Controller
•	Created a new domain name “CyberNet.lab”

<img width="468" height="217" alt="image" src="https://github.com/user-attachments/assets/71f9b39e-4d68-4d6f-92a3-dbd6887ffaff" />

 
Didn’t use advanced mode here. Did later in screenshots for delegation on OUs.



Step 2 – Creation of Organizational Units (Ous)
Even though OUs were initially created I decide to create my own.
•	Created Ous for Users, Admin and Computers to organize objects and simplify administration

<img width="468" height="203" alt="image" src="https://github.com/user-attachments/assets/4a7e4e6f-b364-4e71-ad37-73d3a492e731" />




Step 3. Creating Users and Groups
•	Created user and admin accounts like Kaleb B and Kester B
•	Created admin and user groups “Admins” and “Help Desk”
•	Added Kester B to “Admins” and Kaleb B to “Help Desk” 
  
<img width="468" height="199" alt="image" src="https://github.com/user-attachments/assets/235466df-28f7-485a-aa69-aef8ab4f6415" />

<img width="442" height="264" alt="image" src="https://github.com/user-attachments/assets/a5aff77c-aed7-4714-9893-a24af6431271" />



Step 4. Showing Help Desk Users Permissions & Admins User Permission
•	Delegated permission to Help Desk group so members can create/delete users in CyberNet-Users OU without giving full domain admin rights.
•	Delegated permissions to a single admin user rather than giving full access to all admins added to Admins group
•	Shows effective access Kaleb B is allowed to perform in Level 1 roll
•	Shows effective access Kester B has which is full control in the Admin group
 
 
<img width="468" height="97" alt="image" src="https://github.com/user-attachments/assets/5554ca82-7755-412b-bcb1-3e7c2a580ebe" />

<img width="468" height="239" alt="image" src="https://github.com/user-attachments/assets/ec0b3aa3-5288-4b52-890c-ff3228dacbcf" />





Step 5 – Client Computer Sync
•	Configured client network settings to point to DC as DNS from LAN Server
•	Successful joined “CyberNet.lab”
•	All joined computers will be now moved to CyberNet-computers OU

 
<img width="468" height="233" alt="image" src="https://github.com/user-attachments/assets/ba4bd45a-7982-4e05-adf4-cc683a0a2916" />



Steo 6. Testing
•	Shows Kester B personal workstation has been setup and can now login
•	Screenshots earlier showed working permissions for a single Admin and all CyberNet Users attached to Help Desk

<img width="468" height="243" alt="image" src="https://github.com/user-attachments/assets/f5923634-a328-4b23-b64f-bc54c429e8da" />





Additional screenshots show all three networks are up and running WAN, LAN-SEVER, LAN-CLIENT. Next are all servers are up and running correctly.

<img width="328" height="102" alt="image" src="https://github.com/user-attachments/assets/006c7a0e-85b8-464d-9224-6f58ef136962" />

<img width="468" height="324" alt="image" src="https://github.com/user-attachments/assets/6c2219d7-b50b-40ee-aab9-36258c8c8094" />


  

