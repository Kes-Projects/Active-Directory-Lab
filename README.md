# Active Directory Lab with Windows Server and Windows Clients

## Overview
This project demonstrates the design and deployment of a virtualized Active Directory (AD) environment. The goal is to gain hands-on experience with centralized authentication, user and group management, and policy enforcement in a controlled lab setting.

## Lab Architecture

- **Windows Server 2022** → Domain Controller with Active Directory, DNS, Organizational Units, and Group Policies  
- **Windows 11 Client** → Integrated into the domain for centralized authentication  


## Features Implemented

- Deployed and configured Active Directory domain with DNS, Organizational Units, and Group Policies  
- Created and managed user accounts, security groups, and permissions  
- Integrated Windows clients into the domain for centralized authentication  
- Enforced domain policies across client machines  


## Tools & Technologies

- Windows Server 2022  
- Windows 11  
- Hyper-V / VMware / VirtualBox (virtualization platform of your choice)  

## Future Improvements

- Add additional Windows clients and test group policy deployment at scale  
- Implement automated scripts for user and group management  
- Integrate logging and monitoring with Wazuh or another SIEM tool  
- Simulate real-world scenarios like password policy enforcement or restricted access to shared resources
