
## Step 1. Active Directory Setup
- Installed **Active Directory Domain Services (AD DS)**
- Promoted the server to **Domain Controller**
- Created a new domain: `CyberNet.lab`

<img width="468" height="217" alt="AD Setup" src="https://github.com/user-attachments/assets/71f9b39e-4d68-4d6f-92a3-dbd6887ffaff" />

> Didn’t use advanced mode here. Later screenshots show advanced mode for OU delegation.

---

## Step 2. Creation of Organizational Units (OUs)
Even though default OUs were created, I decided to create my own custom OUs.

- Created OUs for **Users**, **Admins**, and **Computers** to organize objects and simplify administration.

<img width="468" height="203" alt="OU Creation" src="https://github.com/user-attachments/assets/4a7e4e6f-b364-4e71-ad37-73d3a492e731" />

---

## Step 3. Creating Users and Groups
- Created user and admin accounts such as **Kaleb B** and **Kester B**.
- Created groups: **Admins** and **Help Desk**.
- Added **Kester B** to the *Admins* group and **Kaleb B** to the *Help Desk* group.

<img width="468" height="199" alt="Users and Groups" src="https://github.com/user-attachments/assets/235466df-28f7-485a-aa69-aef8ab4f6415" />

<img width="442" height="264" alt="Group Membership" src="https://github.com/user-attachments/assets/a5aff77c-aed7-4714-9893-a24af6431271" />

---

## Step 4. Delegating Permissions
- Delegated permissions to the **Help Desk** group so members can create/delete users in the `CyberNet-Users` OU without granting full domain admin rights.
- Delegated permissions to a single admin user, instead of giving all admins unrestricted control.
- Verified **effective access**:
  - **Kaleb B** (Help Desk) → Limited permissions
  - **Kester B** (Admin) → Full control

<img width="468" height="97" alt="Delegation" src="https://github.com/user-attachments/assets/5554ca82-7755-412b-bcb1-3e7c2a580ebe" />

<img width="468" height="239" alt="Effective Access" src="https://github.com/user-attachments/assets/ec0b3aa3-5288-4b52-890c-ff3228dacbcf" />

---

## Step 5. Client Computer Sync
- Configured client network settings to point to the Domain Controller as **DNS** from the LAN server.
- Successfully joined the domain: `CyberNet.lab`.
- Moved joined computers into the `CyberNet-Computers` OU.

<img width="468" height="233" alt="Client Sync" src="https://github.com/user-attachments/assets/ba4bd45a-7982-4e05-adf4-cc683a0a2916" />

---

## Step 6. Testing
- Verified **Kester B**’s workstation login works using domain credentials.
- Earlier screenshots confirmed delegated permissions for the Help Desk group and full permissions for Admins.

<img width="468" height="243" alt="Testing Workstation" src="https://github.com/user-attachments/assets/f5923634-a328-4b23-b64f-bc54c429e8da" />

---

## Additional Verification
- All three networks (**WAN**, **LAN-Server**, **LAN-Client**) are up and running.
- All servers are operating correctly.

<img width="328" height="102" alt="Networks" src="https://github.com/user-attachments/assets/006c7a0e-85b8-464d-9224-6f58ef136962" />

<img width="468" height="324" alt="Servers Running" src="https://github.com/user-attachments/assets/6c2219d7-b50b-40ee-aab9-36258c8c8094" />

---
